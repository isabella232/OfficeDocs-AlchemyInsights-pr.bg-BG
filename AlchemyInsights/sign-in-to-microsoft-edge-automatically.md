---
title: Автоматично влизане в Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676831"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="1ccbc-102">Автоматично влизане в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1ccbc-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="1ccbc-103">Microsoft Edge използва акаунтът по подразбиране на операционната система, за да записва автоматично потребителя според това как е конфигурирано устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="1ccbc-104">По-долу са описани сценариите за всеки тип конфигурация на устройства и неговия зависим потребителски процес за влизане:</span><span class="sxs-lookup"><span data-stu-id="1ccbc-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="1ccbc-105">**Устройството е хибридно/пад-J**: тази опция е налична в Windows 10, на ниво Windows и съответните версии на сървъра.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="1ccbc-106">Потребителите се подписват автоматично със своите акаунти за Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="1ccbc-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="1ccbc-107">**Устройството е регистрирано по домейни**: тази опция е налична в Windows 10, на ниво Windows и съответните версии на сървъра.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="1ccbc-108">По подразбиране потребителите със акаунти за домейни не се подписват автоматично; за да разрешите автоматичното влизане за тях, използвайте правилата за **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="1ccbc-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="1ccbc-109">За да разрешите автоматичното влизане за потребители с акаунти за Azure AD, обмислете хибридно свързване на устройствата.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="1ccbc-110">**Акаунтът по подразбиране на операционната система е акаунт в Microsoft**: тази опция е налична в Windows 10 RS3 (версия 1709, компилация 10.0.16299) и по-нови версии.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="1ccbc-111">Сценарият е невероятно да се появява на корпоративни устройства.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="1ccbc-112">Ако обаче акаунтът по подразбиране на операционната система е акаунт в Microsoft, Microsoft Edge автоматично ще влезе в акаунта на потребителя с акаунт в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1ccbc-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
