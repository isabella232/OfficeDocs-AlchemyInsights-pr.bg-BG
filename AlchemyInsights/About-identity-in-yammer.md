---
title: За самоличността в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148171"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="84366-102">За самоличността в Yammer</span><span class="sxs-lookup"><span data-stu-id="84366-102">About identity in Yammer</span></span>

<span data-ttu-id="84366-103">Препоръчва се всички мрежи да предприемат следните стъпки, за да се избегнат свързани с идентичността проблеми:</span><span class="sxs-lookup"><span data-stu-id="84366-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="84366-104">Прилагане на Office 365 самоличност след осигуряване на акаунти в Microsoft 365 за потребители в Azure AD да се гарантира, че всички потребители влизат с помощта на основния си акаунт в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="84366-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="84366-105">За повече информация вижте [прилагане на office 365 самоличност за Yammer потребители](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="84366-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="84366-106">Консолидиране на няколко yammer мрежи.</span><span class="sxs-lookup"><span data-stu-id="84366-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="84366-107">Стари Yammer конфигурации позволяват няколко Yammer мрежи да бъде свързан към един клиент.</span><span class="sxs-lookup"><span data-stu-id="84366-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="84366-108">За повече информация вижте [Миграция на мрежата - консолидиране на множество мрежи Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="84366-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="84366-109">По желание на прилагането на лицензиране за Yammer да блокирате потребители от Yammer, ако нямат лиценз.</span><span class="sxs-lookup"><span data-stu-id="84366-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="84366-110">За повече информация вижте [управление на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="84366-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="84366-111">Накрая проверка на списъка на потребителите за по-стари мрежи на Yammer и спиране на стари потребители.</span><span class="sxs-lookup"><span data-stu-id="84366-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="84366-112">Препоръчва се да преустановите (деактивирате) потребителите, вместо да ги изтривате, защото изтриването е необратимо.</span><span class="sxs-lookup"><span data-stu-id="84366-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="84366-113">За повече информация вижте [Проверка на Yammer потребители в мрежи, свързани към Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) и [премахване на потребители](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="84366-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="84366-114">Като конфигурирате Yammer чрез тези стъпки, ще бъдете готови да конфигурирате вашата Yammer мрежа за основен режим за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="84366-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="84366-115">За повече информация вижте [Конфигуриране на вашата Yammer мрежа за основен режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="84366-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>