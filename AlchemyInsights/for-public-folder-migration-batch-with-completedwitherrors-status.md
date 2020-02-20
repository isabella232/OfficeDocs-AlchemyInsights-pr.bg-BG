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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="577d8-102">За публична папка партида за мигриране с завършенос грешки състояние</span><span class="sxs-lookup"><span data-stu-id="577d8-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="577d8-103">Използвайте следните стъпки, за да завършите папката, пропускане на големи/лоши елементи:</span><span class="sxs-lookup"><span data-stu-id="577d8-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="577d8-104">Одобийте пропуснатите елементи на партида за мигриране:</span><span class="sxs-lookup"><span data-stu-id="577d8-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="577d8-105">Използвайте следната команда, за да одобрите пропуснати тела на мигриране на заявки, които са "Синхронизирани", но не е завършена:</span><span class="sxs-lookup"><span data-stu-id="577d8-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="577d8-106">Партида за мигриране и заявки трябва да възобнови и завърши след няколко минути.</span><span class="sxs-lookup"><span data-stu-id="577d8-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

