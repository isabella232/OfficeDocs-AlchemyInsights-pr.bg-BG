---
title: Отстраняване на неизправности при отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505368"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="63dbd-102">Отстраняване на неизправности в достъпа отказан съобщения в Центъра за администриране на Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="63dbd-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="63dbd-103">Ако получавате съобщение за отказан достъп при опит за преглед на центъра за администриране на Sharepoint/OneDrive, уверете се, че [сте присволи лиценз на потребителя](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="63dbd-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="63dbd-104">Ако потребителят има лиценз, трябва също така да се уверите, че му е [присвоена роля](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) на администратор, който може да получи достъп до центровете за администриране.</span><span class="sxs-lookup"><span data-stu-id="63dbd-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="63dbd-105">Този проблем може да възникне, когато потребителят се изтрива и създава отново със същото основно име на потребителя (UPN).</span><span class="sxs-lookup"><span data-stu-id="63dbd-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="63dbd-106">Новият акаунт се създава с различна стойност puid (паспорт уникален ИД).</span><span class="sxs-lookup"><span data-stu-id="63dbd-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="63dbd-107">Когато потребителят се опита да получите достъп до колекция от сайтове или своя OneDrive, потребителят е неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="63dbd-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="63dbd-108">Втори сценарий включва указатели с Active Directory организационна единица (ОЕ).</span><span class="sxs-lookup"><span data-stu-id="63dbd-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="63dbd-109">Ако потребителите вече са влезли в SharePoint и след това се преместват в друг ОЕ и resynced SharePoint, те може да се появи този проблем.</span><span class="sxs-lookup"><span data-stu-id="63dbd-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="63dbd-110">За да разрешите този проблем, трябва да възстановите първоначалната UPN стъпки в статията, [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="63dbd-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="63dbd-111">Забележка: Ако OneDrive или център за администриране на SharePoint не е наличен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.</span><span class="sxs-lookup"><span data-stu-id="63dbd-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="63dbd-112">[Проверете таблото за състояние на услугата](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="63dbd-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


