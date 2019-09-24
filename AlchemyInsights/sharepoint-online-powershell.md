---
title: SharePoint online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122988"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="60d59-102">SharePoint online PowerShell</span><span class="sxs-lookup"><span data-stu-id="60d59-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="60d59-103">Работа с PowerShell или скриптове в SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="60d59-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="60d59-104">За повече информация посетете връзките по-долу.</span><span class="sxs-lookup"><span data-stu-id="60d59-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="60d59-105">Запознаване с онлайн обвивката за управление на SharePoint</span><span class="sxs-lookup"><span data-stu-id="60d59-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="60d59-106">Свързване със спо-PowerShell с многофакторно удостоверяване (МФП)</span><span class="sxs-lookup"><span data-stu-id="60d59-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="60d59-107">[Моделите и практиките на SharePoint (ПНП)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) съдържат библиотека от команди на PowerShell, която ви позволява да извършвате комплексни управленски действия към спо.</span><span class="sxs-lookup"><span data-stu-id="60d59-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="60d59-108">Ако имате проблеми при свързването с обвивката за управление на спо, уверете се, че сте актуализирани до най-новата версия и опитайте да [импортирате отново модула](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) с помощта на *"Import-модул Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="60d59-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="60d59-109">Ако се опитвате да стартирате клиентски обектен модел скриптове, ще трябва да имате [SharePoint online клиентски компоненти SDK](https://www.microsoft.com/download/details.aspx?id=42038) инсталиран на вашия локален компютър.</span><span class="sxs-lookup"><span data-stu-id="60d59-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="60d59-110">Ако имате проблеми при изпълнение на скриптове от PowerShell, може да искате да обмислите изпълнението на PowerShell като администратор и промяна на [правилата за изпълнение](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="60d59-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>