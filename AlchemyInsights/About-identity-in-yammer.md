---
title: За самоличността в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664159"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="672ff-102">За самоличността в Yammer</span><span class="sxs-lookup"><span data-stu-id="672ff-102">About identity in Yammer</span></span>

<span data-ttu-id="672ff-103">Препоръчва се всички мрежи да предприемат следните стъпки, за да се избегнат проблеми, свързани с самоличността:</span><span class="sxs-lookup"><span data-stu-id="672ff-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="672ff-104">Използвайте самоличността на Office 365, след като осигурите акаунтите за Microsoft 365 за потребители в Azure AD, за да сте сигурни, че всички потребители ще влизат, като използват основния си акаунт за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="672ff-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="672ff-105">За повече информация вижте [прилагане на самоличността на Office 365 за потребители на Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="672ff-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="672ff-106">Консолидиране на няколко мрежи Yammer.</span><span class="sxs-lookup"><span data-stu-id="672ff-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="672ff-107">Наследени конфигурации на Yammer разрешават много мрежи на Yammer да бъдат свързани с един клиент.</span><span class="sxs-lookup"><span data-stu-id="672ff-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="672ff-108">За повече информация вижте [мрежа за мигриране – консолидиране на няколко мрежи Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="672ff-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="672ff-109">Ако желаете, можете да наложите лицензиране за Yammer, за да блокирате потребители от Yammer, ако нямат лиценз.</span><span class="sxs-lookup"><span data-stu-id="672ff-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="672ff-110">За повече информация вижте [управление на потребителските лицензи за Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="672ff-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="672ff-111">И накрая, Претърсете списъка с потребители за по-стари мрежи на Yammer и преустановявайте наследени потребители.</span><span class="sxs-lookup"><span data-stu-id="672ff-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="672ff-112">Препоръчително е да прекратите (дезактивирате) потребители, вместо да ги изтривате, тъй като изтриването е необратимо.</span><span class="sxs-lookup"><span data-stu-id="672ff-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="672ff-113">За повече информация вижте [проверка на потребителите на Yammer в мрежите, свързани с Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) , и [Премахване на потребители](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="672ff-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="672ff-114">Чрез конфигуриране на Yammer с помощта на тези стъпки ще можете също да конфигурирате своята мрежа на Yammer за основен режим за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="672ff-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="672ff-115">За повече информация вижте [Конфигуриране на вашата мрежа на Yammer за роден режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="672ff-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>