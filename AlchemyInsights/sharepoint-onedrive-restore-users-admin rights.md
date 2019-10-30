---
title: Отстраняване на неизправности достъп отказан съобщения OneDrive за бизнес сайтове
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766700"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="55064-102">Отстраняване на неизправности достъп отказан съобщения OneDrive за бизнес сайтове</span><span class="sxs-lookup"><span data-stu-id="55064-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="55064-103">Този проблем най-често се случва, когато потребител се изтрива и създава отново със същото основно потребителско име (UPN).</span><span class="sxs-lookup"><span data-stu-id="55064-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="55064-104">Нов акаунт се създава с помощта на различен PUID (паспорт Еднозначен ID) стойност.</span><span class="sxs-lookup"><span data-stu-id="55064-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="55064-105">Когато потребителят се опита да получите достъп до колекция от сайтове или техните OneDrive, потребителят е неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="55064-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="55064-106">Втори сценарий включва указатели с Active Directory организационна единица (ОЕ).</span><span class="sxs-lookup"><span data-stu-id="55064-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="55064-107">Ако потребителите вече са влезли в SharePoint и след това се преместват в друга ОЕ и повторно синхронизиране с SharePoint, те могат да възникнат този проблем.</span><span class="sxs-lookup"><span data-stu-id="55064-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="55064-108">За да разрешите този проблем, трябва да възстановите оригиналния UPN стъпки в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="55064-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="55064-109">Ако не можете да възстановите първоначалния потребител трябва да премахнете стария потребител от сайта на OneDrive с помощта на тези стъпки, [премахнете потребител от списъка с информация за потребителя]().</span><span class="sxs-lookup"><span data-stu-id="55064-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="55064-110">След това се прави, можете да проверите потребителят има администраторски права на сайта на OneDrive като следвате стъпките за добавяне на [администратор за onedrive на потребителя](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="55064-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="55064-111">За повече информация относно нивата на разрешение вижте статията, [разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="55064-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
