---
title: Политика за защита на молбите
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423295"
---
# <a name="application-protection-policy"></a><span data-ttu-id="26193-102">Политика за защита на молбите</span><span class="sxs-lookup"><span data-stu-id="26193-102">Application protection policy</span></span>

<span data-ttu-id="26193-103">Ако сте нови за правилата за защита на приложението (APP), разгледайте преглед на [правилата за защита](https://docs.microsoft.com/intune/apps/app-protection-policy)на приложения .</span><span class="sxs-lookup"><span data-stu-id="26193-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="26193-104">За да започнете да използвате ПРИЛОЖЕНИЕТО, вижте [Как да създадете и присвоите правила за защита на приложенията](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="26193-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="26193-105">Изисквания на политиката за защита на приложението:</span><span class="sxs-lookup"><span data-stu-id="26193-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="26193-106">Потребителят има лиценз Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="26193-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="26193-107">Потребителят принадлежи към група, насочена към правилата за защита на приложението.</span><span class="sxs-lookup"><span data-stu-id="26193-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="26193-108">Само един корпоративен потребител е влязъл в защитени приложения на дадено устройство.</span><span class="sxs-lookup"><span data-stu-id="26193-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="26193-109">Приложението е внедрило [sdK На Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="26193-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="26193-110">За списък с приложения, които поддържат SDK, вижте [защитените с Microsoft Intune приложения.](https://docs.microsoft.com/intune/apps-supported-intune-apps)</span><span class="sxs-lookup"><span data-stu-id="26193-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="26193-111">Правилата важат, след като потребител, който отговаря на горните изисквания, се регистрира в приложение с активирано Внтуе SDK.</span><span class="sxs-lookup"><span data-stu-id="26193-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="26193-112">Най-лесният начин да определите дали се прилага дадена политика е като се изисква потребителят да зададе ПИН в правилата.</span><span class="sxs-lookup"><span data-stu-id="26193-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="26193-113">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="26193-113">For more information, see:</span></span>

[<span data-ttu-id="26193-114">ЧЗВ за отстраняване на НЕИЗПРАВНОСТИ APP/MAM</span><span class="sxs-lookup"><span data-stu-id="26193-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="26193-115">Как да проверите настройката на правилата за защита на приложението</span><span class="sxs-lookup"><span data-stu-id="26193-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="26193-116">Разберете времето за доставка на правилата за защита на приложението</span><span class="sxs-lookup"><span data-stu-id="26193-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="26193-117">Как да следите правилата за защита на приложения</span><span class="sxs-lookup"><span data-stu-id="26193-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)