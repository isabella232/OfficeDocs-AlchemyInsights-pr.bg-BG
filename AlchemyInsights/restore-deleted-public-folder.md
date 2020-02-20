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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158480"
---
# <a name="restore-a-deleted-public-folder"></a>Възстановяване на изтрита публична папка

**За да възстановите изтритите елементи от публична папка:**

- Вижте Не можете да възстановите изтрити елементи от публична папка за [поща в Outlook 2016](https://aka.ms/pfrec).
 
**За да възстановите изтрита публична папка (от произволен тип):** 

- Използвайте следната команда EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример: Следната команда ще възстанови Subfolder1 и ще го постави под \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

За повече подробности вижте [Възстановяване на изтрита публична папка.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
