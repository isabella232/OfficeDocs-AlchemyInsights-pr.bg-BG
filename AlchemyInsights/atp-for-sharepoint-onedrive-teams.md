---
title: ATP за SharePoint, OneDrive и Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715550"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="9c5fc-102">ATP за SharePoint, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9c5fc-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="9c5fc-103">Следвайте тези стъпки, за да разрешите разширена защита от заплахи:</span><span class="sxs-lookup"><span data-stu-id="9c5fc-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="9c5fc-104">Отидете на [https://protection.office.com](https://protection.office.com) и влезте с акаунт на глобален администратор или администратор на защитата.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="9c5fc-105">В левия навигационния екран под **управление на заплахи**изберете **Policy** \> **безопасни прикачени файлове**за правилата.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="9c5fc-106">Изберете **включване на ATP за SharePoint, OneDrive и Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="9c5fc-107">[Създайте политика за предупреждения за дейността](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , за да получавате известия, когато откриваме злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="9c5fc-108">За пълни инструкции вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9c5fc-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="9c5fc-109">**Забележка**: по проект ATP не преглежда всеки отделен файл в SharePoint Online, OneDrive за бизнеса или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="9c5fc-110">Файловете се сканират асинхронно чрез процес, който използва дейността за споделяне, дейността за гост и сигнали със заплахи за идентифициране на злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="9c5fc-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="9c5fc-111">За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9c5fc-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
