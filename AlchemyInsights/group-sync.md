---
title: Синхронизиране на група
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256668"
---
# <a name="group-sync"></a><span data-ttu-id="c0e2a-102">Синхронизиране на група</span><span class="sxs-lookup"><span data-stu-id="c0e2a-102">Group sync</span></span>

<span data-ttu-id="c0e2a-103">Тази статия предоставя указания за груповите синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c0e2a-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="c0e2a-104">Ако глобален администратор или собственик на група не е в състояние да модифицира свойствата на групата или да добави членове или да присвоява собственици в портала на Azure, се уверете, че източникът на органа за групата е Azure Active Directory (Azure AD) за глобалния администратор или собственика на групата, за да модифицирате групата.</span><span class="sxs-lookup"><span data-stu-id="c0e2a-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="c0e2a-105">Преди да се опитате да изтриете синхронизирана група в Azure AD, уверете се, че сте [изтрили всички присвоени лицензи](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) , за да избегнете грешки.</span><span class="sxs-lookup"><span data-stu-id="c0e2a-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="c0e2a-106">За да разберете как да синхронизирате потребители, групи и контакти, вижте [Синхронизиране на AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)и следвайте [синхронизирането на локална група в Azure с ПОМОЩТА на Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) , за да синхронизирате групи с помощта на ad Connect.</span><span class="sxs-lookup"><span data-stu-id="c0e2a-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="c0e2a-107">Следвайте това ръководство [отстраняване на грешки по време на синхронизация](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) за отстраняване на често срещани грешки по време на синхронизация.</span><span class="sxs-lookup"><span data-stu-id="c0e2a-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

