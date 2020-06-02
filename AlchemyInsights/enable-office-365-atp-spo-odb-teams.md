---
title: Разрешаване на Office 365 ATP за екипи на SharePoint, OneDrive и Microsoft
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506907"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1c80e-102">Разрешаване на разширена защита срещу заплахи за Office 365 за SharePoint Online, OneDrive и екипи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="1c80e-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1c80e-103">Отидете на https://protection.office.com и влезте в профила си.</span><span class="sxs-lookup"><span data-stu-id="1c80e-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1c80e-104">Изберете **Правила за управление на**  >  **Policy**  >  **заплахите Безопасни прикачени файлове**.</span><span class="sxs-lookup"><span data-stu-id="1c80e-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1c80e-105">Изберете **Включване на ATP за SharePoint, OneDrive и Екипи на Microsoft**, след което щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="1c80e-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1c80e-106">(Препоръчително) Като глобален администратор или SharePoint Online администратор, стартирайте кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedFileDownload** настроен на *true.*</span><span class="sxs-lookup"><span data-stu-id="1c80e-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1c80e-107">(Препоръчително) [Настройване на предупреждения](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.</span><span class="sxs-lookup"><span data-stu-id="1c80e-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1c80e-108">ATP ще сканира всеки отделен файл в SharePoint Online, OneDrive или екипи на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1c80e-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1c80e-109">Файловете се сканират асинхронно, чрез процес, който използва събития за споделяне и гост дейност, заедно с интелигентни евристични методи и заплахи за идентифициране на злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="1c80e-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1c80e-110">Вижте [ATP за SharePoint, OneDrive и Екипи на Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="1c80e-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>