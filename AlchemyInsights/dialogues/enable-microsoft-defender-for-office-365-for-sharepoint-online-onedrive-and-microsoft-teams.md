---
title: Разрешаване на Microsoft Defender за Office 365 за SharePoint Online, OneDrive и Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692620"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3f35c-102">Разрешаване на Microsoft Defender за Office 365 за SharePoint Online, OneDrive и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3f35c-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="3f35c-103">Като използвате своя глобален администратор или идентификационни данни на администратор на защита, влезте в [центъра за защита и съответствие на Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="3f35c-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="3f35c-104">Изберете **управление на заплахите** в левия екран и след това изберете  >  [безопасни прикачени файлове](https://protection.office.com/safeattachment)за правилата.</span><span class="sxs-lookup"><span data-stu-id="3f35c-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="3f35c-105">Изберете **включване на Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams** и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="3f35c-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="3f35c-106">Като глобален администратор или администратор на SharePoint Online, изпълнете следната кратка команда на PowerShell с параметъра **DisallowInfectedFileDownload** , зададен на *TRUE*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="3f35c-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="3f35c-107">Настройване на известявания за открити файлове</span><span class="sxs-lookup"><span data-stu-id="3f35c-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="3f35c-108">За повече информация вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="3f35c-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
