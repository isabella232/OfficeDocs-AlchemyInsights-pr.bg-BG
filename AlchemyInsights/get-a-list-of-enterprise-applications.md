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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404232"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="1a652-102">Получаване на списък с корпоративни приложения</span><span class="sxs-lookup"><span data-stu-id="1a652-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="1a652-103">За **да получите списък с** корпоративни приложения (всички приложения или филтрирани по Показвано име, ИД, URI за идентификатори и т.н.) чрез командата Powershell, вижте [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="1a652-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="1a652-104">За да получите списък на основните обекти на услугата (всички обекти или филтрирани по ИД) чрез командата Powershell, вижте [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="1a652-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="1a652-105">Ако искате да получите **списък с конфигурирани от SAML приложения, следните скриптове на PowerShell може да** ви помогнат:</span><span class="sxs-lookup"><span data-stu-id="1a652-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="1a652-106">Всяко приложение е приложението OAuth или SAML приложение (както галерия, така и приложения, които не са галерия), ще имат два обекта, създадени в AAD, когато се случи регистрацията им.</span><span class="sxs-lookup"><span data-stu-id="1a652-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="1a652-107">Единият се нарича обект на приложение, а другият е обектът главен на услугата.</span><span class="sxs-lookup"><span data-stu-id="1a652-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="1a652-108">Когато захвърлите свойствата на главен обект на услугата с помощта на PowerShell, ще откриете, че всяко приложение има определен брой етикети, свързани с него, като:</span><span class="sxs-lookup"><span data-stu-id="1a652-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="1a652-109">Приложенията на OAuth ще имат етикет, наречен "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="1a652-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="1a652-110">Галерия SAML Apps ще има етикет, наречен "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="1a652-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="1a652-111">Saml Apps извън галерията ще имат етикет, наречен "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="1a652-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="1a652-112">Следователно можете да използвате тези етикети и да разберете какъв вид приложение е това.</span><span class="sxs-lookup"><span data-stu-id="1a652-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="1a652-113">Етикетът "**WindowsAzureActiveDirectoryIntegratedApp**" е често срещан за всички типове приложения.</span><span class="sxs-lookup"><span data-stu-id="1a652-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="1a652-114">Можете да използвате следния фрагмент, за да изброите всички SAML приложения (както галерия, така и не галерия):</span><span class="sxs-lookup"><span data-stu-id="1a652-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="1a652-115">За повече информация вижте Идентифициране [на приложения, разрешени чрез SAML, в Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="1a652-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="1a652-116">**Намиране и изброяване само на уеб приложения:** Използвайте командата по-долу, за да получите всички приложения на Azure AD с типа на приложението "Уеб приложение/API"</span><span class="sxs-lookup"><span data-stu-id="1a652-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="1a652-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="1a652-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="1a652-118">**Намирайте и изброявайте само основни** приложения: Изпълнете следната команда, за да получите всички приложения за основен клиент (настолно/мобилно устройство).</span><span class="sxs-lookup"><span data-stu-id="1a652-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="1a652-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="1a652-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="1a652-120">**Експортиране на всички регистрирани подробни данни за приложението Azure AD** в CSV файл: Командата по-долу експортира всички приложения на Azure AD с необходимите подробни данни в CSV файл:</span><span class="sxs-lookup"><span data-stu-id="1a652-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="1a652-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="1a652-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="1a652-122">Export-Csv "C:\AzureADApps.csv" – NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="1a652-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="1a652-123">**Трябва да експортирате списък с неизползваните приложения на Azure** – отчет за проверка</span><span class="sxs-lookup"><span data-stu-id="1a652-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="1a652-124">Azure AD може да показва регистрационни файлове на приложения само за до 30 дни, при условие че имате лиценз за Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="1a652-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="1a652-125">Имате две опции за запазване на данните за повече от 30 дни.</span><span class="sxs-lookup"><span data-stu-id="1a652-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="1a652-126">Можете да използвате API за [отчитане на Azure AD,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) за да извличате данните по програмен начин и да ги съхранявате в база данни.</span><span class="sxs-lookup"><span data-stu-id="1a652-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="1a652-127">Като алтернатива можете да интегрирате регистрационните файлове за проверка в SIEM система на трета страна.</span><span class="sxs-lookup"><span data-stu-id="1a652-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="1a652-128">Можете също да изтеглите списъка с приложения за всички приложения и притежавани приложения под Azure Active Directory>Регистрации на приложения>Изтегляне>Всички приложения/притежавани приложения.</span><span class="sxs-lookup"><span data-stu-id="1a652-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="1a652-129">За да получите списък с приложения чрез MS Graph, вижте Списък [на приложенията – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) и тип ресурс на [приложението – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="1a652-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
