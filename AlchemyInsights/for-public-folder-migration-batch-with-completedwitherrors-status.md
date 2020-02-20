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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158587"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>За публична папка партида за мигриране с завършенос грешки състояние

Използвайте следните стъпки, за да завършите папката, пропускане на големи/лоши елементи: 
1. Одобийте пропуснатите елементи на партида за мигриране:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Използвайте следната команда, за да одобрите пропуснати тела на мигриране на заявки, които са "Синхронизирани", но не е завършена:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Партида за мигриране и заявки трябва да възобнови и завърши след няколко минути.

