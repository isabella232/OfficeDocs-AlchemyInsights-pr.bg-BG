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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951122"
---
# <a name="app-registration-owner-issues"></a>Проблеми със собственика на регистрацията на приложения

Следват наличните методи за добавяне на главници като собственици за регистрации на приложения:

- Използване на модула На PowerShell на Azure AD –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Препратка: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Използване на Azure CLI – `az ad app owner add`

    Препратка: [собственик на az ad app](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Използване на ms Graph –

    Справка: [Добавяне на собственик – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Използване на портала на Azure AD – навигиране [до portal.azure.com](https://portal.azure.com/) > Azure Active directory > Регистрация на приложения > Изберете вашето приложение > Собственици > Добавяне на собственици

**Не можете да прегледате вашето приложение в острието за регистрации на приложения, въпреки че сте собственик на това приложение?**

Собственикът на приложение не е административна роля. Ако настройката [Ограничаване на достъпа до портала за администриране на Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) е разрешена, само администраторът ще може да преглежда приложенията в портала за регистрация на приложения. За да може собственикът да преглежда приложенията, забранете тази настройка (Задайте това на НЕ) или да присвоите роля на администратор на собственика само за конкретното приложение. За тази цел обаче ще ви трябва лиценз за Azure AD Premium P2 и да [разрешите Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
