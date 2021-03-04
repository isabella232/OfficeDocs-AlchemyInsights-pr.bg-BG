---
title: Наблюдение на настройките за условен достъп
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427056"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="f2168-102">Наблюдение на настройките за условен достъп</span><span class="sxs-lookup"><span data-stu-id="f2168-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="f2168-103">Потребителите, които са насочени към условен достъп, ще получат имейл за известяване, ако не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="f2168-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f2168-104">За да разрешите, ви препоръчваме едно или няколко от следните решения:</span><span class="sxs-lookup"><span data-stu-id="f2168-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="f2168-105">Ако устройството се предполага, че е записано, уведомете потребителя да отиде в приложението Company Portal и да се увери, че той се появява във фирмения портал.</span><span class="sxs-lookup"><span data-stu-id="f2168-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f2168-106">Ако не е, потребителят трябва да запише устройството.</span><span class="sxs-lookup"><span data-stu-id="f2168-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="f2168-107">В портала на Azure отидете на **Настройки** за  >  **съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="f2168-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="f2168-108">За да видите отчета за съответствие на устройството, за да се уверите, че устройството на потребителя е маркирано като съвместимо, под **наблюдение** щракнете върху **съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="f2168-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="f2168-109">В портала на Azure отидете на **Настройки** за  >  **съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="f2168-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="f2168-110">Под **управление** щракнете върху **правила**.</span><span class="sxs-lookup"><span data-stu-id="f2168-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="f2168-111">В списъка с правила за съответствие Проверете дали даден профил е присвоен на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="f2168-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f2168-112">Ако не е присвоен профил, в противен случай няма да може да се потвърди състоянието на съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="f2168-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="f2168-113">Редактирайте възложената задача за условен достъп на потребителя.</span><span class="sxs-lookup"><span data-stu-id="f2168-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="f2168-114">В портала на Azure се придвижете до **Настройване** на правила за  >  **условен достъп**  >  , изберете политика от списъка и щракнете върху **потребители и групи**.</span><span class="sxs-lookup"><span data-stu-id="f2168-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="f2168-115">За да насочвате определени правила към някого, добавете ги към **списъка включване**.</span><span class="sxs-lookup"><span data-stu-id="f2168-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="f2168-116">За да се гарантира, че даден човек е пропуснат от правилата, добавете ги към **списъка за изключване**.</span><span class="sxs-lookup"><span data-stu-id="f2168-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="f2168-117">**Полезни връзки:**</span><span class="sxs-lookup"><span data-stu-id="f2168-117">**Helpful links:**</span></span>

- [<span data-ttu-id="f2168-118">Общ преглед на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="f2168-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="f2168-119">Отстраняване на неизправности при CA</span><span class="sxs-lookup"><span data-stu-id="f2168-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="f2168-120">Правила за отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="f2168-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="f2168-121">Следене на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="f2168-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="f2168-122">Тези стъпки са полезни само при отстраняване на неизправности с функцията за условен достъп на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f2168-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="f2168-123">Възможно е също така да поставите под карантина устройството блокирането на имейл достъпа чрез правилата за Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2168-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="f2168-124">Повече информация за управлението на устройства на Exchange можете да намерите [**тук**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="f2168-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
