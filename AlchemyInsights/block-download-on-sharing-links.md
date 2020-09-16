---
title: Блокиране на изтеглянето чрез връзките за споделяне
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685731"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="17144-102">Блокиране на изтеглянето чрез връзките за споделяне</span><span class="sxs-lookup"><span data-stu-id="17144-102">Block download on sharing links</span></span>

<span data-ttu-id="17144-103">**Блок изтеглянето** е достъпно за **връзки само за преглед** към документи на Office.</span><span class="sxs-lookup"><span data-stu-id="17144-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="17144-104">Когато изберете тази опция, хората, които получат достъп до файла чрез създадената от вас връзка, няма да виждат опции за изтегляне, отпечатване или копиране на файла.</span><span class="sxs-lookup"><span data-stu-id="17144-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="17144-105">Администраторите могат да управляват дали настройката "блокиране на изтеглянето" се появява само за файлове на Office или не чрез промяна на `BlockDownloadLinksFileType` настройката в кратките команди [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) или [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17144-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
