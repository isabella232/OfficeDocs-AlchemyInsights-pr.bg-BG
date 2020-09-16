---
title: Папка за мигриране на публични папки със статус CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744102"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Папка за мигриране на публични папки със статус CompletedWithErrors

Използвайте следните стъпки, за да завършите партидата, като пропуснете големите/лошите елементи: 
1. Одобряване на пропуснатите елементи в партида за мигриране:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Използвайте командата по-долу, за да одобрите пропуснатите елементи в искания за мигриране, които са "синхронизирани", но не са изпълнени:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Партидата за мигриране и исканията трябва да се възобновят и допълнят за няколко минути.

