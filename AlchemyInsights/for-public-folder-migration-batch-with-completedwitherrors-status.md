---
title: За публична папка партида за мигриране с завършенос грешки състояние
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043567"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>За публична папка партида за мигриране с завършенос грешки състояние

Използвайте следните стъпки, за да завършите папката, пропускане на големи/лоши елементи: 
1. Одобийте пропуснатите елементи на партида за мигриране:

    Задаване на \<партида партида партида миграция>-ApproveSkippedItems 
2. Използвайте следната команда, за да одобрите пропуснати тела на мигриране на заявки, които са "Синхронизирани", но не е завършена:

    $pf=Получаване-публичнапапкаMailboxМиграцияискане | Get-publicFolderMailboxМиграциязаявкастатистика -включваотчет; ЗаВсеки ($i в $pf) {ако ($i.LargeItemsEncountered -gt 0 -или $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxМиграцияИскане за миграция$i.ИдентифициращGuid -Прескачане на елементОдобрениеTime ([Дата и час]::Utcnow}}
3. Партида за мигриране и заявки трябва да възобнови и завърши след няколко минути.

