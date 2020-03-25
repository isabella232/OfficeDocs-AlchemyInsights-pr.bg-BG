---
title: Съветите за правилата на DLP не работят
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932575"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="aff41-102">Проблеми с правилото за DLP</span><span class="sxs-lookup"><span data-stu-id="aff41-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="aff41-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="aff41-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="aff41-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="aff41-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="aff41-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="aff41-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="aff41-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="aff41-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="aff41-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="aff41-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="aff41-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="aff41-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="aff41-109">**Съвети за правила на DLP**</span><span class="sxs-lookup"><span data-stu-id="aff41-109">**DLP policy tips**</span></span>

<span data-ttu-id="aff41-110">Когато използвате **DLP правила**, потребителите могат да бъдат уведомени за нарушение на правилата с **правилата съвети**.</span><span class="sxs-lookup"><span data-stu-id="aff41-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="aff41-111">Администраторите могат да конфигурират съвети за правилата за показване, докато тестват техните DLP правила или когато правилата са в режим на пълно прилагане.</span><span class="sxs-lookup"><span data-stu-id="aff41-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="aff41-112">За да конфигурирате правила съвети за правилата на DLP в центъра за защита и съответствие в режим на пълно прилагане, направете следното:</span><span class="sxs-lookup"><span data-stu-id="aff41-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="aff41-113">Уверете се, че съветите за правила са **разрешени** за DLP правилото, като използвате стъпките [тук](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="aff41-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="aff41-114">Уверете се, че съдържанието ви **съответства** на това, което е **необходимо** за задействане на правилото, описано в тази статия [тук](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="aff41-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="aff41-115">Съвети за правилата се показват в OWA и Outlook.</span><span class="sxs-lookup"><span data-stu-id="aff41-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="aff41-116">Обаче при използване на **Outlook 2013 или по-нова**, съвети за правила се показват само при определени условия.</span><span class="sxs-lookup"><span data-stu-id="aff41-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="aff41-117">Тези условия са изброени тук: [Поддържани условия за Outlook 2013 или по-късно за показване на правила съвети](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="aff41-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="aff41-118">За допълнителна информация относно съветите за dlp правила вижте: [Показвай съвети за правила за DLP правила](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="aff41-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  