---
title: Разрешаване на Office 365 ATP за SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709896"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c5961-102">Разрешаване на разширена защита от заплахи за Office 365 за SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c5961-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c5961-103">Отидете на https://protection.office.com и влезте.</span><span class="sxs-lookup"><span data-stu-id="c5961-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c5961-104">Изберете **Threat management**за  >  **Policy**  >  **безопасни прикачени файлове**към политиката за управление на заплахи.</span><span class="sxs-lookup"><span data-stu-id="c5961-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c5961-105">Изберете **включване на ATP за SharePoint, OneDrive и Microsoft Teams**и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="c5961-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c5961-106">Препоръчва Като глобален администратор или администратор на SharePoint Online, изпълнете кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с набора от параметри **DisallowInfectedFileDownload** на *TRUE*.</span><span class="sxs-lookup"><span data-stu-id="c5961-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c5961-107">Препоръчва [Настройване на известявания](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.</span><span class="sxs-lookup"><span data-stu-id="c5961-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c5961-108">ATP ще сканира всеки отделен файл в SharePoint Online, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c5961-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c5961-109">Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и дейността за гост, както и интелигентни евристики и сигнали със заплахи за идентифициране на злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="c5961-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c5961-110">Вижте [ATP за SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c5961-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>