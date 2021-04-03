---
title: Възстановяване на изтрита група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505671"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="b6770-102">Възстановяване на изтрита група на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b6770-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="b6770-103">Можете да възстановите изтрита група на Microsoft 365 или Microsoft Teams в рамките на 30 дни от изтриването.</span><span class="sxs-lookup"><span data-stu-id="b6770-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="b6770-104">За да влезете в центъра за администриране на Microsoft 365 и да изброите изтритите групи и екипи, отидете в центъра за администриране на [Microsoft 365](https://aka.ms/RestoreDeletedGroup).</span><span class="sxs-lookup"><span data-stu-id="b6770-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="b6770-105">**Забележка:** Влезте с помощта на акаунта, който е присвоен на администратора на клиента или ролята на администратор на групите.</span><span class="sxs-lookup"><span data-stu-id="b6770-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="b6770-106">Изберете изтритата група на Microsoft 365/Teams, която да бъде възстановена, и щракнете върху **групата за възстановяване.**</span><span class="sxs-lookup"><span data-stu-id="b6770-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="b6770-107">Ако групата не може да бъде възстановена поради конфликтен SMTP адрес, използвайте следната команда, за да намерите обекта, който причинява конфликт, и премахнете SMTP адреса:</span><span class="sxs-lookup"><span data-stu-id="b6770-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="b6770-108">**Забележка:** В някои случаи може да отнеме до 24 часа, докато групата и всичките й данни бъдат възстановени.</span><span class="sxs-lookup"><span data-stu-id="b6770-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="b6770-109">За повече информация или за да научите как да възстановявате групи с помощта на PowerShell, вижте [Възстановяване на изтрита група на Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="b6770-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>