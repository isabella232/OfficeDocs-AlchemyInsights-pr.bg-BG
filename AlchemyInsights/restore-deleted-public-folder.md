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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="df857-102">Възстановяване на изтрита публична папка</span><span class="sxs-lookup"><span data-stu-id="df857-102">Restore a deleted public folder</span></span>

<span data-ttu-id="df857-103">**За да възстановите изтритите елементи от публична папка:**</span><span class="sxs-lookup"><span data-stu-id="df857-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="df857-104">Вижте Не можете да възстановите изтрити елементи от публична папка за [поща в Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="df857-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="df857-105">**За да възстановите изтрита публична папка (от произволен тип):**</span><span class="sxs-lookup"><span data-stu-id="df857-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="df857-106">Използвайте следната команда EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="df857-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="df857-107">Синтаксис:</span><span class="sxs-lookup"><span data-stu-id="df857-107">Syntax:</span></span>

    ><span data-ttu-id="df857-108">$pf=Вземи-публична папка \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Име -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-път, където папката ще бъде възстановена></span><span class="sxs-lookup"><span data-stu-id="df857-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="df857-109">Пример: Следната команда ще възстанови Subfolder1 и ще го постави под \Parent1:</span><span class="sxs-lookup"><span data-stu-id="df857-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="df857-110">$pf=Вземи-публична папка \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Име -eq "Subfolder1"}; Задаване на публична папка $pf.identity -път \parent1</span><span class="sxs-lookup"><span data-stu-id="df857-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="df857-111">За повече подробности вижте [Възстановяване на изтрита публична папка.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="df857-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
