---
title: Източник на обвивка на Sharepoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764250"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fca4d-102">Източник на обвивка на Sharepoint</span><span class="sxs-lookup"><span data-stu-id="fca4d-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fca4d-103">Работа с PowerShell или скриптове в Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="fca4d-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fca4d-104">Посетете връзките по-долу за повече информация.</span><span class="sxs-lookup"><span data-stu-id="fca4d-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fca4d-105">Първи стъпки с онлайн обвивката за управление на SharePoint</span><span class="sxs-lookup"><span data-stu-id="fca4d-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fca4d-106">Свързване към SPO PowerShell с многофакторно удостоверяване (МВНР)</span><span class="sxs-lookup"><span data-stu-id="fca4d-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fca4d-107">[Моделите и практиките на SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) съдържа библиотека с команди на PowerShell, която ви позволява да извършвате сложни действия за управление на SPO.</span><span class="sxs-lookup"><span data-stu-id="fca4d-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fca4d-108">Ако имате проблеми при свързване с обвивката за управление на SPO, уверете се, че сте актуализирали до най-новата версия и опитайте [да импортирате отново модула](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) с *помощта на "Импортиране модул microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="fca4d-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fca4d-109">Ако се опитвате да изпълните клиентски обектен модел скриптове, трябва да имате [Sharepoint Online клиентски компоненти SDK](https://www.microsoft.com/download/details.aspx?id=42038) инсталиран на вашия локален компютър.</span><span class="sxs-lookup"><span data-stu-id="fca4d-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fca4d-110">Ако имате проблеми с изпълнението на скриптове от PowerShell, можете да помислите за изпълнение на PowerShell като администратор и промяна на [правилата за изпълнение](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="fca4d-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>