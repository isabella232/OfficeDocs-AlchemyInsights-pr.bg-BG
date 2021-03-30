---
title: Проблеми със собственика на регистрацията на приложения
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404213"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="34551-102">Проблеми със собственика на регистрацията на приложения</span><span class="sxs-lookup"><span data-stu-id="34551-102">App Registration Owner issues</span></span>

<span data-ttu-id="34551-103">Следват наличните методи за добавяне на главници като собственици за регистрации на приложения:</span><span class="sxs-lookup"><span data-stu-id="34551-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="34551-104">Използване на модула На PowerShell на Azure AD –</span><span class="sxs-lookup"><span data-stu-id="34551-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="34551-105">Препратка: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="34551-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="34551-106">Използване на Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="34551-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="34551-107">Препратка: [собственик на az ad app](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="34551-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="34551-108">Използване на MS Graph –</span><span class="sxs-lookup"><span data-stu-id="34551-108">Using MS Graph -</span></span>

    <span data-ttu-id="34551-109">Справка: [Добавяне на собственик – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="34551-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="34551-110">Използване на портала на Azure AD – навигиране [до portal.azure.com](https://portal.azure.com/) > Azure Active directory > Регистрация на приложения > Изберете вашето приложение > Собственици > Добавяне на собственици</span><span class="sxs-lookup"><span data-stu-id="34551-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="34551-111">**Не можете да прегледате вашето приложение в острието за регистрации на приложения, въпреки че сте собственик на това приложение?**</span><span class="sxs-lookup"><span data-stu-id="34551-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="34551-112">Собственикът на приложение не е административна роля.</span><span class="sxs-lookup"><span data-stu-id="34551-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="34551-113">Ако настройката [Ограничаване на достъпа до портала за администриране на Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) е разрешена, само администраторът ще може да преглежда приложенията в портала за регистрация на приложения.</span><span class="sxs-lookup"><span data-stu-id="34551-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="34551-114">За да може собственикът да преглежда приложенията, забранете тази настройка (Задайте това на НЕ) или да присвоите роля на администратор на собственика само за конкретното приложение.</span><span class="sxs-lookup"><span data-stu-id="34551-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="34551-115">За тази цел обаче ще ви е необходим лиценз за Azure AD Premium P2 и ще разрешите управлението на [привилегирована самоличност.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="34551-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
