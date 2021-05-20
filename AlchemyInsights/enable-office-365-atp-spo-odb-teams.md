---
title: Разрешаване Office 365 ATP за SharePoint, OneDrive и Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543917"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="eefda-102">Разрешаване на Microsoft Defender за Office 365 за SharePoint онлайн, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eefda-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="eefda-103">Отидете и https://protection.office.com влезте.</span><span class="sxs-lookup"><span data-stu-id="eefda-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="eefda-104">Изберете **Правила за управление на**  >  **заплахи** Сейф прикачени  >  **файлове**.</span><span class="sxs-lookup"><span data-stu-id="eefda-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="eefda-105">Изберете **Включване на защитника за Office 365 за SharePoint, OneDrive и Microsoft Teams** и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="eefda-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="eefda-106">(Препоръчва се) Като глобален администратор или администратор на SharePoint Online изпълнете кратката команда [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedFileDownload,** зададен на *true*.</span><span class="sxs-lookup"><span data-stu-id="eefda-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="eefda-107">(Препоръчва се) [Настройване на известия за](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) открити файлове.</span><span class="sxs-lookup"><span data-stu-id="eefda-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="eefda-108">Microsoft Defender за Office 365 няма да сканира всеки един файл в SharePoint Онлайн, OneDrive или Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eefda-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="eefda-109">Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и дейности за гости, както и интелигентни уравнения и сигнали за заплахи за идентифициране на злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="eefda-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="eefda-110">Вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="eefda-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>