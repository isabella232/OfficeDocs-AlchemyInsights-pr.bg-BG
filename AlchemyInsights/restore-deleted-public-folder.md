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
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809428"
---
# <a name="restore-a-deleted-public-folder"></a>Възстановяване на изтрита публична папка

**За да възстановите изтрити елементи от публична папка:**

- Вижте Не можете да възстановите изтрити елементи от публична папка, която не [е в пощата, в Outlook 2016](https://aka.ms/pfrec).
 
**За да възстановите изтрита публична папка (от всякакъв тип):** 

- Използвайте следната команда EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример: Следната команда ще възстанови подпапка1 и ще я постави под \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Вижте [Възстановяване на изтрита публична папка](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) за повече подробности.
