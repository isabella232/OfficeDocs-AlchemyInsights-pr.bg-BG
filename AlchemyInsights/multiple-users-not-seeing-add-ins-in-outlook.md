---
title: Много потребители не виждат добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729860"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ccf66-102">Много потребители не виждат добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="ccf66-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ccf66-103">Ако тествате добавки на Outlook и нито едно не се показва, като първа стъпка за отстраняване на неизправности, използвайте кратката команда **get-OrganizationConfig** PowerShell, за да заявите параметъра _AppsForOfficeEnabled_ .</span><span class="sxs-lookup"><span data-stu-id="ccf66-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="ccf66-104">Ако заявката връща стойност **FALSE**, настройте този параметър на **TRUE** с помощта на кратката команда **Set-OrganizationConfig** , така че добавките да се показват по очаквания начин.</span><span class="sxs-lookup"><span data-stu-id="ccf66-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="ccf66-105">Не препоръчваме параметърът _AppsForOfficeEnabled_ е зададен на **FALSE**.</span><span class="sxs-lookup"><span data-stu-id="ccf66-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="ccf66-106">Стойността на **FALSE** отменя всички настройки по-горе за администриране и потребители и позволява на всички нови приложения да бъдат активирани от всеки потребител в организацията.</span><span class="sxs-lookup"><span data-stu-id="ccf66-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="ccf66-107">За повече информация вижте [Задаване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="ccf66-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>