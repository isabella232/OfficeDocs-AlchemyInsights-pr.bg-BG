---
title: Възстановяване на изтрита публична папка
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
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943364"
---
# <a name="restore-a-deleted-public-folder"></a>Възстановяване на изтрита публична папка

**За да възстановите изтрити елементи от публична папка:**

- Вижте Не можете да възстановите изтрити елементи от публична папка, която не е [поща, в Outlook 2016](https://aka.ms/pfrec).
 
**За да възстановите изтрита публична папка (от всякакъв тип):** 

- Използвайте следната команда EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример: Следната команда ще възстанови подпапка1 и ще я постави под \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Вижте [Възстановяване на изтрита публична папка](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) за повече подробности.
