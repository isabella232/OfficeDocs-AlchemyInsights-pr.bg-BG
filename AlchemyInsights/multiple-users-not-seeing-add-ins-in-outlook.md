---
title: Много потребители, които не виждат добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197737"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="9f61d-102">Много потребители, които не виждат добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="9f61d-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="9f61d-103">Ако тествате Outlook добавки и никой не се появи, като първата стъпка за отстраняване на неизправности, използвайте кратката команда **Get-OrganizationConfig** PowerShell да _заявката за параметъра AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="9f61d-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="9f61d-104">Ако заявката връща стойност на **false**, задайте този параметър **true** чрез кратката команда **Set-OrganizationConfig,** така добавки се появяват според очакванията.</span><span class="sxs-lookup"><span data-stu-id="9f61d-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="9f61d-105">Не препоръчваме параметърът _AppsForOfficeEnabled_ да е зададен **на False.**</span><span class="sxs-lookup"><span data-stu-id="9f61d-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="9f61d-106">Стойността на **False** отменя всички горепосочени административни и потребителски настройки за роли и предотвратява активирането на всички нови приложения от всеки потребител в организацията.</span><span class="sxs-lookup"><span data-stu-id="9f61d-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="9f61d-107">За повече информация вж. [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="9f61d-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>