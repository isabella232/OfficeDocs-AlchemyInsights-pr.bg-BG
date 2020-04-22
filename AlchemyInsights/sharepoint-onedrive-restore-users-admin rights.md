---
title: Отстраняване на отказан достъп съобщения до OneDrive за бизнес сайтове
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692790"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e772f-102">Отстраняване на отказан достъп съобщения до OneDrive за бизнес сайтове</span><span class="sxs-lookup"><span data-stu-id="e772f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e772f-103">Този проблем най-често възниква, когато потребител се изтрива и създава отново с едно и също основно потребителско име (UPN).</span><span class="sxs-lookup"><span data-stu-id="e772f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e772f-104">Новият акаунт се създава чрез различна стойност на PUID (уникален ид на паспорт).</span><span class="sxs-lookup"><span data-stu-id="e772f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e772f-105">Когато потребителят се опита да получите достъп до колекция от сайтове или oneDrive, потребителят има неправилен PUID.</span><span class="sxs-lookup"><span data-stu-id="e772f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e772f-106">Втори сценарий включва синхронизиране на директории с Active Directory организационна единица (ОЕ).</span><span class="sxs-lookup"><span data-stu-id="e772f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e772f-107">Ако потребителите вече са влезли в SharePoint и след това се преместват в друг OU и resynced с SharePoint, те могат да възникнат този проблем.</span><span class="sxs-lookup"><span data-stu-id="e772f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e772f-108">За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в статията, [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e772f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="e772f-109">Ако не можете да възстановите първоначалния потребител, трябва да премахнете стария потребител от oneDrive сайт, като използвате тези стъпки, [Премахнете потребител от списъка с информация за потребителя]().</span><span class="sxs-lookup"><span data-stu-id="e772f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e772f-110">След това е направено, можете да проверите потребителят има администраторски права на сайта oneDrive, като следвате стъпките [за Добавяне на администратор за OneDrive на потребителя](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="e772f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="e772f-111">За повече информация относно нивата на разрешение вижте [статията, разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="e772f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
