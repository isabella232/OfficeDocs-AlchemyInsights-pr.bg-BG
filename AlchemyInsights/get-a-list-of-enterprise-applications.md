---
title: Получаване на списък с корпоративни приложения
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116717"
---
# <a name="get-a-list-of-enterprise-applications"></a>Получаване на списък с корпоративни приложения

1. За **да получите списък с** корпоративни приложения (всички приложения или филтрирани по Показвано име, ИД, URI за идентификатори и т.н.) чрез командата Powershell, вижте [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. За да получите списък на основните обекти на услугата (всички обекти или филтрирани по ИД) чрез командата Powershell, вижте [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Ако искате да получите **списък с конфигурирани от SAML приложения, следните скриптове на PowerShell може да** ви помогнат:

    Всяко приложение е приложението OAuth или SAML приложение (както галерия, така и приложения, които не са галерия), ще имат два обекта, създадени в AAD, когато се случи регистрацията им. Единият се нарича обект на приложение, а другият е обектът главен на услугата. Когато захвърлите свойствата на главен обект на услугата с помощта на PowerShell, ще откриете, че всяко приложение има определен брой етикети, свързани с него, като:

    - Приложенията на OAuth ще имат етикет, наречен "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Галерия SAML Apps ще има етикет, наречен "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Saml Apps извън галерията ще имат етикет, наречен "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Следователно можете да използвате тези етикети и да разберете какъв вид приложение е това. Етикетът "**WindowsAzureActiveDirectoryIntegratedApp**" е често срещан за всички типове приложения. Можете да използвате следния фрагмент, за да изброите всички SAML приложения (както галерия, така и не галерия):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    За повече информация вижте Идентифициране [на приложения, разрешени чрез SAML, в Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Намиране и изброяване само на уеб приложения:** Използвайте командата по-долу, за да получите всички приложения на Azure AD с типа на приложението "Уеб приложение/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Намирайте и изброявайте само основни** приложения: Изпълнете следната команда, за да получите всички приложения за основен клиент (настолно/мобилно устройство).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Експортиране на всички регистрирани подробни данни за приложението Azure AD** в CSV файл: Командата по-долу експортира всички приложения на Azure AD с необходимите подробни данни в CSV файл:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" – NoTypeInformation -Encoding UTF8

7. **Трябва да експортирате списък с неизползваните приложения на Azure** – отчет за проверка

    Azure AD може да показва регистрационни файлове на приложения само за до 30 дни, при условие че имате лиценз за Azure AD Premium приложение.
    Имате две опции за запазване на данните за повече от 30 дни. Можете да използвате API за [отчитане на Azure AD,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) за да извличате данните по програмен начин и да ги съхранявате в база данни. Като алтернатива можете да интегрирате регистрационните файлове за проверка в SIEM система на трета страна.

    Можете също да изтеглите списъка с приложения за всички приложения и притежавани приложения под Azure Active Directory>Регистрации на приложения>Изтегляне>Всички приложения/притежавани приложения.

    За да получите списък с приложения чрез MS Graph, вижте Списък на [приложенията – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) и тип ресурс [на приложение – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
