---
title: Възстановяване на изтрита публична папка
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063592"
---
# <a name="restore-a-deleted-public-folder"></a>Възстановяване на изтрита публична папка

**За да възстановите изтритите елементи от публична папка:**

- Вижте Не можете да възстановите изтрити елементи от публична папка за [поща в Outlook 2016](https://aka.ms/pfrec).
 
**За да възстановите изтрита публична папка (от произволен тип):** 

- Използвайте следната команда EXO PowerShell:

    Синтаксис:

    >$pf=Вземи-публична папка \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Име -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-път, където папката ще бъде възстановена>

    Пример: Следната команда ще възстанови Subfolder1 и ще го постави под \Parent1:

    >$pf=Вземи-публична папка \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Име -eq "Subfolder1"}; Задаване на публична папка $pf.identity -път \parent1

За повече подробности вижте [Възстановяване на изтрита публична папка.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
