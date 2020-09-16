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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="d1e2b-102">Папка за мигриране на публични папки със статус CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="d1e2b-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="d1e2b-103">Използвайте следните стъпки, за да завършите партидата, като пропуснете големите/лошите елементи:</span><span class="sxs-lookup"><span data-stu-id="d1e2b-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="d1e2b-104">Одобряване на пропуснатите елементи в партида за мигриране:</span><span class="sxs-lookup"><span data-stu-id="d1e2b-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="d1e2b-105">Използвайте командата по-долу, за да одобрите пропуснатите елементи в искания за мигриране, които са "синхронизирани", но не са изпълнени:</span><span class="sxs-lookup"><span data-stu-id="d1e2b-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="d1e2b-106">Партидата за мигриране и исканията трябва да се възобновят и допълнят за няколко минути.</span><span class="sxs-lookup"><span data-stu-id="d1e2b-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

