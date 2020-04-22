---
title: Разрешаване на Office 365 ATP за SharePoint, OneDrive и екипи на Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703415"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fd19c-102">Разрешаване на разширена защита на заплахите за Office 365 за Екипи на SharePoint Online, OneDrive и Microsoft</span><span class="sxs-lookup"><span data-stu-id="fd19c-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="fd19c-103">Отиди https://protection.office.com и се впишете.</span><span class="sxs-lookup"><span data-stu-id="fd19c-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="fd19c-104">Изберете**Правила за** >  **управление на** > **заплахите Безопасни прикачени файлове**.</span><span class="sxs-lookup"><span data-stu-id="fd19c-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="fd19c-105">Изберете **Включване на ATP за SharePoint, OneDrive и Екипи на Microsoft**, след което щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="fd19c-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="fd19c-106">(Препоръчва се) Като глобален администратор или администратор на SharePoint Online изпълнете кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedТаФайлИзтегляне** на *true*.</span><span class="sxs-lookup"><span data-stu-id="fd19c-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="fd19c-107">(Препоръчва се) [Настройване на предупреждения](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.</span><span class="sxs-lookup"><span data-stu-id="fd19c-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="fd19c-108">ATP ще сканира всеки един файл в SharePoint Online, OneDrive или Microsoft Екипи.</span><span class="sxs-lookup"><span data-stu-id="fd19c-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="fd19c-109">Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и активност на гост, заедно с интелигентни евристични и сигнали за заплахи за идентифициране на злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="fd19c-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="fd19c-110">Вижте [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="fd19c-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>