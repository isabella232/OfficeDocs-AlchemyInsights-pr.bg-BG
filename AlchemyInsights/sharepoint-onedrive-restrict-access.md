---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053754"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="5d46c-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="5d46c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="5d46c-103">Има много начини за ограничаване на достъпа до услуги на SharePoint online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5d46c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="5d46c-104">Тези различни методи за ограничаване на достъпа са описани по-долу.</span><span class="sxs-lookup"><span data-stu-id="5d46c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="5d46c-105">**Ограничение на разрешенията**</span><span class="sxs-lookup"><span data-stu-id="5d46c-105">**Permission Restriction**</span></span>

<span data-ttu-id="5d46c-106">В SharePoint online и OneDrive за бизнес ограничаваме достъпа до елементи като сайтове, файлове и папки само чрез предоставяне на достъп до тези групи/лица, които трябва да имат достъп.</span><span class="sxs-lookup"><span data-stu-id="5d46c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="5d46c-107">Персонализиране на разрешенията за списък или библиотека на SharePoint</span><span class="sxs-lookup"><span data-stu-id="5d46c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="5d46c-108">Персонализиране на разрешенията на сайта на SharePoint</span><span class="sxs-lookup"><span data-stu-id="5d46c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="5d46c-109">Промяна на разрешенията на подпапка</span><span class="sxs-lookup"><span data-stu-id="5d46c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="5d46c-110">Контрол на достъпа от неуправлявани устройства</span><span class="sxs-lookup"><span data-stu-id="5d46c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="5d46c-111">Като SharePoint или глобален администратор в Office 365, можете да блокирате или ограничите достъпа до съдържание на SharePoint и OneDrive от неуправлявани устройства (хибридни AD, Съединени или съвместими в InTune).</span><span class="sxs-lookup"><span data-stu-id="5d46c-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="5d46c-112">**Ограничаване на местоположението в мрежата**</span><span class="sxs-lookup"><span data-stu-id="5d46c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="5d46c-113">Като ИТ администратор можете да контролирате достъпа до ресурси на SharePoint и OneDrive въз основа на дефинирани мрежови местоположения, на които имате доверие.</span><span class="sxs-lookup"><span data-stu-id="5d46c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="5d46c-114">Това е известно също като политика, базирана на местоположението.</span><span class="sxs-lookup"><span data-stu-id="5d46c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="5d46c-115">За повече информация вижте [контрол на достъпа до SharePoint online и OneDrive данни въз основа на мрежово местоположение](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="5d46c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="5d46c-116">**Ограничение за заключване на сайта**</span><span class="sxs-lookup"><span data-stu-id="5d46c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="5d46c-117">В SharePoint online имате възможност да заключите колекция от сайтове, така че никой няма достъп.</span><span class="sxs-lookup"><span data-stu-id="5d46c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="5d46c-118">Това е зададено чрез PowerShell и [онлайн обвивката за управление на SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощта на свойството [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -заключване.</span><span class="sxs-lookup"><span data-stu-id="5d46c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="5d46c-119">**Ограничаване на потребителите да създават сайтове или подстраници**</span><span class="sxs-lookup"><span data-stu-id="5d46c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="5d46c-120">Като администратор на SharePoint или Office 365 глобален администратор можете да позволите на потребителите да създават и администрират собствени сайтове на SharePoint, да определят какъв вид сайтове могат да създават и да посочат местоположението на сайтовете.</span><span class="sxs-lookup"><span data-stu-id="5d46c-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="5d46c-121">За повече информация вижте [управление на създаването на сайт в SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="5d46c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

