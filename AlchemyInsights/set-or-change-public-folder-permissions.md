---
title: Задаване или промяна на разрешения за публична папка
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789196"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="c5bd5-102">Разрешения и публични папки</span><span class="sxs-lookup"><span data-stu-id="c5bd5-102">Permissions and Public Folders</span></span>

<span data-ttu-id="c5bd5-103">Можете да промените разрешенията във вашите публични папки с помощта на Outlook, центъра за администриране на Exchange (EAC) или PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c5bd5-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="c5bd5-104">За инструкции на Outlook [щракнете тук](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="c5bd5-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="c5bd5-105">За EAC вижте тази [статия](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) за инструкции.</span><span class="sxs-lookup"><span data-stu-id="c5bd5-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="c5bd5-106">За Powershell вижте тази [статия за инструкции](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) относно използването на Add-PublicFolderClientPermission команда.</span><span class="sxs-lookup"><span data-stu-id="c5bd5-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="c5bd5-107">Ако имате нужда от инструкции за свързване с Exchange Powershell, щракнете [тук](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="c5bd5-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="c5bd5-108">Ако **външни потребители не могат да изпращат** имейли до публична папка с разрешена поща, причината може да е, че публичната папка липсва разрешения, необходими за външно доставяне на имейл.</span><span class="sxs-lookup"><span data-stu-id="c5bd5-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="c5bd5-109">Можете да коригирате това с помощта на [инструкциите на](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)Outlook тук или инструкциите на PowerShell [тук](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="c5bd5-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

