---
title: Проблеми с връзката на SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051702"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="74450-102">Проблеми с връзката на SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="74450-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="74450-103">Ако SharePoint Designer изпитва проблеми с връзката към сайтове на SharePoint, моля, опитайте следните общи решения.</span><span class="sxs-lookup"><span data-stu-id="74450-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="74450-104">Стъпка 1: Проверете дали SharePoint Designer 2013 се актуализира с [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [актуализация на 2 август 2016 за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="74450-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="74450-105">Стъпка 2: изчистете локалните кеш файлове:</span><span class="sxs-lookup"><span data-stu-id="74450-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="74450-106">Затворете SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="74450-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="74450-107">На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.</span><span class="sxs-lookup"><span data-stu-id="74450-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="74450-108">%Pipn%\mimsuser\lucerude</span><span class="sxs-lookup"><span data-stu-id="74450-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="74450-109">%Popon%\mimrosice\larter\sucor</span><span class="sxs-lookup"><span data-stu-id="74450-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="74450-110">%\Usit\up\pulersfir\mupsitep</span><span class="sxs-lookup"><span data-stu-id="74450-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="74450-111">Отворете SharePoint Designer 2013 и въведете отново акаунта, за да видите дали работи.</span><span class="sxs-lookup"><span data-stu-id="74450-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="74450-112">Стъпка 3: [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="74450-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="74450-113">Стъпка 4: администраторите ще трябва да **позволи персонализиран скрипт** в настройките на центъра за администриране на SharePoint, за да позволите на SharePoint Designer връзка.</span><span class="sxs-lookup"><span data-stu-id="74450-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="74450-114">За повече информация вижте [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="74450-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


