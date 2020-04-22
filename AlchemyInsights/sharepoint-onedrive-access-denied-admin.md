---
title: Отстраняване на отказан достъп съобщения
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758364"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="6d456-102">Отстраняване на отказан достъп съобщения в центъра за администриране на SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="6d456-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="6d456-103">Ако получавате съобщение за отказан достъп при опит за преглед на център за администриране на Sharepoint/OneDrive, моля, уверете се, че [присвоите лиценз на потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="6d456-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="6d456-104">Ако потребителят има лиценз, трябва също да се уверите, че им е [присвоена администраторска роля,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) която да има достъп до центровете за администриране.</span><span class="sxs-lookup"><span data-stu-id="6d456-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="6d456-105">Този проблем може да възникне, когато потребител е изтрит и повторно създаден със същото основно потребителско име (UPN).</span><span class="sxs-lookup"><span data-stu-id="6d456-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="6d456-106">Новият акаунт се създава чрез различна стойност на PUID (уникален ид на паспорт).</span><span class="sxs-lookup"><span data-stu-id="6d456-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="6d456-107">Когато потребителят се опита да получите достъп до колекция от сайтове или oneDrive, потребителят има неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="6d456-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="6d456-108">Втори сценарий включва синхронизиране на директории с Active Directory организационна единица (ОЕ).</span><span class="sxs-lookup"><span data-stu-id="6d456-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="6d456-109">Ако потребителите вече са влезли в SharePoint и след това се преместват в друг OU и resynced с SharePoint, те могат да възникнат този проблем.</span><span class="sxs-lookup"><span data-stu-id="6d456-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="6d456-110">За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в [статията, възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6d456-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="6d456-111">Забележка: Ако OneDrive или център за администриране на SharePoint не е достъпен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.</span><span class="sxs-lookup"><span data-stu-id="6d456-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="6d456-112">[Проверете таблото за изправност на услугата](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6d456-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


