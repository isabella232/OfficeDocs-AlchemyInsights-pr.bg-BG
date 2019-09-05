---
title: Отстраняване на съобщения за отказан достъп
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751265"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="7c2fe-102">Отстраняване на съобщения за отказан достъп в SharePoint/OneDrive център за администриране</span><span class="sxs-lookup"><span data-stu-id="7c2fe-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="7c2fe-103">Ако получавате съобщение за отказан достъп при опит за преглеждане в център за администриране на SharePoint/OneDrive, моля, уверете се, че [присвоявате лиценз на потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="7c2fe-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="7c2fe-104">Ако потребителят има лиценз, трябва да се уверите, че те са [присвоени администраторски роля](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , която има достъп до центровете за администриране.</span><span class="sxs-lookup"><span data-stu-id="7c2fe-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="7c2fe-105">Този проблем може да възникне, когато потребителят се изтрива и създава отново със същото основно потребителско име (UPN).</span><span class="sxs-lookup"><span data-stu-id="7c2fe-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7c2fe-106">Нов акаунт се създава с помощта на различен PUID (паспорт Еднозначен ID) стойност.</span><span class="sxs-lookup"><span data-stu-id="7c2fe-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7c2fe-107">Когато потребителят се опита да получите достъп до колекция от сайтове или техните OneDrive, потребителят е неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="7c2fe-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7c2fe-108">Втори сценарий включва указатели с Active Directory организационна единица (ОЕ).</span><span class="sxs-lookup"><span data-stu-id="7c2fe-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7c2fe-109">Ако потребителите вече са влезли в SharePoint и след това се преместват в друга ОЕ и повторно синхронизиране с SharePoint, те могат да възникнат този проблем.</span><span class="sxs-lookup"><span data-stu-id="7c2fe-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="7c2fe-110">За да разрешите този проблем, трябва да възстановите оригиналния UPN стъпки в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="7c2fe-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="7c2fe-111">Забележка: Ако OneDrive или център за администриране на SharePoint не е достъпен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.</span><span class="sxs-lookup"><span data-stu-id="7c2fe-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="7c2fe-112">[Проверете таблото за изправността на услугата](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7c2fe-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


