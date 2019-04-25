---
title: Разрешаване на Office 365 АТФ за SharePoint, OneDrive и екипи на Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403022"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="d591a-102">Разрешаване на Office 365 разширени заплаха защита за SharePoint онлайн, OneDrive и екипи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="d591a-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="d591a-103">Отидете на https://protection.office.com и влезте в нея.</span><span class="sxs-lookup"><span data-stu-id="d591a-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="d591a-104">Изберете **управление на заплахите** > **политика** > **Безопасно прикачени файлове**.</span><span class="sxs-lookup"><span data-stu-id="d591a-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="d591a-105">Изберете **включване на АТФ за SharePoint, OneDrive и екипи на Microsoft**и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="d591a-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="d591a-106">(Препоръчва се) Като глобален администратор или администратор на SharePoint Online стартирате кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **DisallowInfectedFileDownload** параметър, зададен на *true*.</span><span class="sxs-lookup"><span data-stu-id="d591a-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="d591a-107">(Препоръчва се) [Настройка на предупрежденията](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за откритите файлове.</span><span class="sxs-lookup"><span data-stu-id="d591a-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="d591a-108">ATP ще НОТ сканиране всеки един файл в SharePoint Online, OneDrive или екипи на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d591a-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="d591a-109">Файлове се сканират асинхронно, чрез процес, който използва споделяне и гост дейност събития, умни евристики и заплахата сигнали, за да идентифицира злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="d591a-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="d591a-110">Вижте [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d591a-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>