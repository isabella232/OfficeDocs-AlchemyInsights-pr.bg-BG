---
title: PowerShell на SharePoint online
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786878"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="0ea05-102">PowerShell на SharePoint online</span><span class="sxs-lookup"><span data-stu-id="0ea05-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="0ea05-103">Работите с PowerShell или скриптове в SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="0ea05-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="0ea05-104">Посетете връзките по-долу за повече информация.</span><span class="sxs-lookup"><span data-stu-id="0ea05-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="0ea05-105">Първи стъпки в обвивката за управление на SharePoint online</span><span class="sxs-lookup"><span data-stu-id="0ea05-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="0ea05-106">Свързване към "с"</span><span class="sxs-lookup"><span data-stu-id="0ea05-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="0ea05-107">[Модели и практики на SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) съдържат библиотека с команди на PowerShell, която ви позволява да извършвате сложни управленски дейности към "за".</span><span class="sxs-lookup"><span data-stu-id="0ea05-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="0ea05-108">Ако имате проблеми със свързването на обвивката за управление на за доставяне, уверете се, че сте актуализирали до най-новата версия и се опитайте да [импортирате отново модула](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) с помощта на *"Import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="0ea05-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="0ea05-109">Ако се опитвате да изпълнявате скриптове за модели на обекти на клиент, ще трябва да имате инсталиран [SDK на компонента за клиент на SharePoint online](https://www.microsoft.com/download/details.aspx?id=42038) на вашия локален компютър.</span><span class="sxs-lookup"><span data-stu-id="0ea05-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="0ea05-110">Ако имате проблеми при изпълнението на скриптове от PowerShell, може да поискате да помислите за изпълнение на PowerShell като администратор и да промените [правилата за изпълнение](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="0ea05-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>