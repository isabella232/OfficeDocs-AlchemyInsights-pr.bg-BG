---
title: Разполагане на Microsoft Edge за мобилни устройства за iOS/iPadOS или Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/11/2020
ms.locfileid: "49676927"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="29547-102">Разполагане на Microsoft Edge за мобилни устройства за iOS/iPadOS или Android</span><span class="sxs-lookup"><span data-stu-id="29547-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="29547-103">Примерът с упътвания, обобщен по-долу, ще ви помогне да присвоите Microsoft Edge на потребители на устройства с iOS, iPadOS и Android.</span><span class="sxs-lookup"><span data-stu-id="29547-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="29547-104">След като изпълните тези стъпки, правилата за настройване на Microsoft ще позволят следните функции на Microsoft Edge за бизнеса:</span><span class="sxs-lookup"><span data-stu-id="29547-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="29547-105">Dual самоличност</span><span class="sxs-lookup"><span data-stu-id="29547-105">Dual identity</span></span>
- <span data-ttu-id="29547-106">Интегриране с правилата за защита на приложения на Microsoft</span><span class="sxs-lookup"><span data-stu-id="29547-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="29547-107">Интегриране с прокси сървър на приложението Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="29547-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="29547-108">Управлявани предпочитани и клавишни комбинации за началната страница</span><span class="sxs-lookup"><span data-stu-id="29547-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="29547-109">Ако сте блокирали потребители да записва мобилни устройства, този сценарий с упътвания няма да работи и потребителите ще трябва сами да инсталират Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="29547-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="29547-110">За да разположите Microsoft Edge за Mobile за iOS/iPadOS или Android, вижте:</span><span class="sxs-lookup"><span data-stu-id="29547-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="29547-111">Предпоставки</span><span class="sxs-lookup"><span data-stu-id="29547-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="29547-112">Въвеждането</span><span class="sxs-lookup"><span data-stu-id="29547-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="29547-113">Основите</span><span class="sxs-lookup"><span data-stu-id="29547-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="29547-114">Конфигуриране</span><span class="sxs-lookup"><span data-stu-id="29547-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="29547-115">Възложени задачи</span><span class="sxs-lookup"><span data-stu-id="29547-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="29547-116">Преглед и създаване</span><span class="sxs-lookup"><span data-stu-id="29547-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
