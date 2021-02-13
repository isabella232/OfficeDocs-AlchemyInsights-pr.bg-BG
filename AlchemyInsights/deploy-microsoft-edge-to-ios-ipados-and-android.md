---
title: Разполагане на Microsoft Edge за iOS, iPadOS и Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194453"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="b7359-102">Разполагане на Microsoft Edge за iOS, iPadOS и Android</span><span class="sxs-lookup"><span data-stu-id="b7359-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="b7359-103">Примерът с упътвания, обобщен по-долу, ще ви помогне да присвоите Microsoft Edge на потребители на устройства с iOS, iPadOS и Android.</span><span class="sxs-lookup"><span data-stu-id="b7359-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="b7359-104">Ако сте блокирали потребители да записва мобилни устройства, този сценарий с упътвания няма да работи и потребителите ще трябва сами да инсталират Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b7359-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="b7359-105">Примерът с упътвания включва следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="b7359-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="b7359-106">Предпоставки</span><span class="sxs-lookup"><span data-stu-id="b7359-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="b7359-107">Въвеждането</span><span class="sxs-lookup"><span data-stu-id="b7359-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="b7359-108">Основите</span><span class="sxs-lookup"><span data-stu-id="b7359-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="b7359-109">Конфигуриране</span><span class="sxs-lookup"><span data-stu-id="b7359-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="b7359-110">Възложени задачи</span><span class="sxs-lookup"><span data-stu-id="b7359-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="b7359-111">Преглед и създаване</span><span class="sxs-lookup"><span data-stu-id="b7359-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="b7359-112">След като приключите със стъпките в указания сценарий, правилата за настройване на Microsoft ще позволят следните функции на Microsoft Edge за бизнеса:</span><span class="sxs-lookup"><span data-stu-id="b7359-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="b7359-113">Dual самоличност</span><span class="sxs-lookup"><span data-stu-id="b7359-113">Dual identity</span></span>
- <span data-ttu-id="b7359-114">Интегриране с правилата за защита на приложения на Microsoft</span><span class="sxs-lookup"><span data-stu-id="b7359-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="b7359-115">Интегриране с прокси сървър на приложението Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b7359-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="b7359-116">Управлявани предпочитани и клавишни комбинации за началната страница</span><span class="sxs-lookup"><span data-stu-id="b7359-116">Managed favorites and home page shortcuts</span></span>
