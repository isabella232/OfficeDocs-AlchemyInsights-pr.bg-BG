---
title: Отстраняване на неизправности при проблеми със собственик
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900759"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="3624b-102">Отстраняване на неизправности при проблеми със собственик</span><span class="sxs-lookup"><span data-stu-id="3624b-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="3624b-103">За да отстраните проблеми, свързани със собственика, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="3624b-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="3624b-104">[Добавяне или промяна на администратори на абонаменти за Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): групите на Azure Active Directory (Azure ad) се притежават и се управляват от собственици на групи.</span><span class="sxs-lookup"><span data-stu-id="3624b-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="3624b-105">Собствениците на групи могат да бъдат потребители или ръководители на услуги и могат да управляват групата, включително членството.</span><span class="sxs-lookup"><span data-stu-id="3624b-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="3624b-106">Само съществуващи собственици на група или група управляващи администраторите могат да присвояват собственици на групи.</span><span class="sxs-lookup"><span data-stu-id="3624b-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="3624b-107">Собствениците на групи не са задължени да членуват в групата.</span><span class="sxs-lookup"><span data-stu-id="3624b-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="3624b-108">[Добавяне или промяна на администратори на абонаменти за Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): тази статия описва как да добавите или промените ролята на администратор за потребител, ИЗПОЛЗВАЩ Azure RBAC, в обхвата на абонамента.</span><span class="sxs-lookup"><span data-stu-id="3624b-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="3624b-109">Използвайте PowerShell, за да добавите собственик на група или собственик на приложение.</span><span class="sxs-lookup"><span data-stu-id="3624b-109">Use PowerShell to add a group owner or an application owner.</span></span>
