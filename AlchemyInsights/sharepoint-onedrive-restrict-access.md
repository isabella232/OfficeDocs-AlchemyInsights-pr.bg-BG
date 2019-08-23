---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559866"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7e141-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="7e141-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7e141-103">Има много начини за ограничаване на достъпа до услуги SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7e141-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="7e141-104">Тези различни методи за ограничаване на достъп са описани по-долу.</span><span class="sxs-lookup"><span data-stu-id="7e141-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="7e141-105">**Разрешение ограничение**</span><span class="sxs-lookup"><span data-stu-id="7e141-105">**Permission Restriction**</span></span>

<span data-ttu-id="7e141-106">В SharePoint Online и OneDrive за бизнес ограничаваме достъпа до обекти като сайтове, файлове и папки чрез само предоставяне на достъп до тези групи/лица, които трябва да имат достъп.</span><span class="sxs-lookup"><span data-stu-id="7e141-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="7e141-107">Персонализиране на разрешения за списък на SharePoint или библиотека</span><span class="sxs-lookup"><span data-stu-id="7e141-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="7e141-108">Персонализиране на разрешения на сайт на SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e141-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="7e141-109">Промяна на разрешенията на подпапка</span><span class="sxs-lookup"><span data-stu-id="7e141-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="7e141-110">Контрол на достъпа от неуправляван устройства</span><span class="sxs-lookup"><span data-stu-id="7e141-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="7e141-111">Като SharePoint или глобален администратор в Office 365, можете да блокирате или да ограничите достъпа до съдържание на SharePoint и OneDrive от неуправляван устройства (тези не хибрид АД се присъединиха или съвместими в Intune).</span><span class="sxs-lookup"><span data-stu-id="7e141-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="7e141-112">**Мрежа местоположение ограничение**</span><span class="sxs-lookup"><span data-stu-id="7e141-112">**Network Location Restriction**</span></span>

<span data-ttu-id="7e141-113">Като ИТ администратор можете да контролирате достъпа до SharePoint и OneDrive ресурси, на базата на определени мрежови местоположения, които имате доверие.</span><span class="sxs-lookup"><span data-stu-id="7e141-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="7e141-114">Това е също така известен като местоположение базирани политика.</span><span class="sxs-lookup"><span data-stu-id="7e141-114">This is also known as location-based policy.</span></span> <span data-ttu-id="7e141-115">За повече информация моля вижте [контрол на достъпа до SharePoint Online и OneDrive данни, базиращи се на местоположение в мрежата](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="7e141-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="7e141-116">**Ограничението за заключване на сайта**</span><span class="sxs-lookup"><span data-stu-id="7e141-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="7e141-117">В рамките на SharePoint Online имате възможност за заключване надолу колекция сайтове, така че никой няма достъп.</span><span class="sxs-lookup"><span data-stu-id="7e141-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="7e141-118">Това се задава чрез PowerShell и [SharePoint онлайн управление Шел](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) използване на [Набор-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState собственост.</span><span class="sxs-lookup"><span data-stu-id="7e141-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="7e141-119">**Ограничаване на потребителите да създават сайтове, или подсайтове**</span><span class="sxs-lookup"><span data-stu-id="7e141-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="7e141-120">Като администратор на SharePoint или Office 365 е глобален администратор, можете да позволите на вашите потребители създават и управляват свои собствени сайтове на SharePoint, определи какви сайтове те могат да създават и Задайте местоположението на обектите.</span><span class="sxs-lookup"><span data-stu-id="7e141-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="7e141-121">За повече информация моля вижте [управление създаването на сайт в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="7e141-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

