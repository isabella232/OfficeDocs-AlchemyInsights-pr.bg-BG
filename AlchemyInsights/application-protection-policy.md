---
title: Правила за защита на приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716882"
---
# <a name="application-protection-policy"></a><span data-ttu-id="dc9c2-102">Правила за защита на приложения</span><span class="sxs-lookup"><span data-stu-id="dc9c2-102">Application protection policy</span></span>

<span data-ttu-id="dc9c2-103">Ако сте начинаещ в правилата за защита на приложения (приложението), вижте [общ преглед на правилата за защита на приложения](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="dc9c2-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="dc9c2-104">За да започнете да използвате приложението, вижте [как да създавате и присвоявате правила за защита на приложения](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="dc9c2-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="dc9c2-105">Изисквания за правила за защита на приложения:</span><span class="sxs-lookup"><span data-stu-id="dc9c2-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="dc9c2-106">Потребителят има лиценз за администратор или EMS.</span><span class="sxs-lookup"><span data-stu-id="dc9c2-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="dc9c2-107">Потребителят принадлежи към група, която е предназначена за правилата за защита на приложения.</span><span class="sxs-lookup"><span data-stu-id="dc9c2-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="dc9c2-108">Само един корпоративен потребител е влязъл в защитени приложения на устройство.</span><span class="sxs-lookup"><span data-stu-id="dc9c2-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="dc9c2-109">Приложението е въвело добавката [SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="dc9c2-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="dc9c2-110">За списък с приложения, които поддържат SDK, вижте [защитени приложения на Microsoft](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="dc9c2-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="dc9c2-111">Правилата важат, след като потребител, който отговаря на посочените по-горе изисквания, влезе в приложение за настройване на SDK.</span><span class="sxs-lookup"><span data-stu-id="dc9c2-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="dc9c2-112">Най-лесният начин да определите дали е приложено правило, като изисква потребителят да зададе PIN код в правилата.</span><span class="sxs-lookup"><span data-stu-id="dc9c2-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="dc9c2-113">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="dc9c2-113">For more information, see:</span></span>

[<span data-ttu-id="dc9c2-114">ЧЗВ за отстраняване на неизправности с приложения/MAM</span><span class="sxs-lookup"><span data-stu-id="dc9c2-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="dc9c2-115">Как да проверите настройката на правилата за защита на вашите приложения</span><span class="sxs-lookup"><span data-stu-id="dc9c2-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="dc9c2-116">Разберете времето за доставяне на правилата за защита на приложения</span><span class="sxs-lookup"><span data-stu-id="dc9c2-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="dc9c2-117">Как се проследяват правилата за защита на приложения</span><span class="sxs-lookup"><span data-stu-id="dc9c2-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)