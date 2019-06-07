---
title: Отстраняване на неизправности при съобщения за отказан достъп
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760330"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ad4df-102">Отстраняване на неизправности при съобщения за отказан достъп в центъра за администриране на Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="ad4df-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ad4df-103">Ако получавате съобщение за отказан, когато се опитвате да отидете до центъра за администриране на Sharepoint/OneDrive достъп, моля уверете се, че можете да [присвоите даден лиценз за потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="ad4df-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="ad4df-104">Ако потребителят има лиценз, ти рамо също правя сигурен те са [възложени на администратор роля](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) която достъп на администратор центрове.</span><span class="sxs-lookup"><span data-stu-id="ad4df-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="ad4df-105">Този въпрос също може да възникне, когато потребителят е изтрита и създадена отново със същото основно име на потребителя (UPN).</span><span class="sxs-lookup"><span data-stu-id="ad4df-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ad4df-106">Новият акаунт е създаден с помощта на различни PUID (паспорт уникален ИД) стойност.</span><span class="sxs-lookup"><span data-stu-id="ad4df-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ad4df-107">Когато потребителят се опитва да получи достъп до колекция от сайтове или техните OneDrive, потребителят има неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="ad4df-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ad4df-108">Вторият сценарий включва директория синхронизация с Active Directory организационни единици (OU).</span><span class="sxs-lookup"><span data-stu-id="ad4df-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ad4df-109">Ако потребителите са вече влезли в SharePoint, след това се премества в различни OU и resynced с SharePoint, те могат да срещнат този проблем.</span><span class="sxs-lookup"><span data-stu-id="ad4df-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ad4df-110">За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ad4df-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="ad4df-111">Забележка: Ако OneDrive или SharePoint администратор център не е наличен на множество потребители, които преди това са имали достъп, може да има проблем при временна услуга.</span><span class="sxs-lookup"><span data-stu-id="ad4df-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ad4df-112">[Проверете услуги здравето на таблото](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ad4df-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


