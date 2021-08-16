---
title: За партида за мигриране на публични папки със състояние "Завършенисъсerrors"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068153"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>За партида за мигриране на публични папки със състояние "Завършенисъсerrors"

Използвайте следните стъпки, за да завършите партидата, като прескочите големите/лошите елементи: 
1. Одобряване на пропуснати елементи в партидата за мигриране:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Използвайте следната команда, за да одобрите пропуснати елементи в искания за мигриране, които са "Синхронизирани", но не са изпълнени:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Партидата за мигриране и исканията трябва да се възобновят и довършат след няколко минути.

