---
title: Лимитът на ежедневните имейли е превишен. Работният поток е спрян.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053106"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="232c2-103">Ограничение на дневния имейл лимит.</span><span class="sxs-lookup"><span data-stu-id="232c2-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="232c2-104">Работният поток е спрян.</span><span class="sxs-lookup"><span data-stu-id="232c2-104">Workflow is suspended.</span></span>

<span data-ttu-id="232c2-105">Тази грешка може да бъде получена в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="232c2-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="232c2-106">Имате работен поток в SharePoint Online, използващ SharePoint 2010 или SharePoint 2013 работен поток платформа тип.</span><span class="sxs-lookup"><span data-stu-id="232c2-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="232c2-107">Работният поток е конфигуриран да изпраща потребителски имейл съобщение до повече от 200 потребители наведнъж, повече от 10 000 получатели на ден, или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="232c2-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="232c2-108">Когато стартирате работния поток, имейл съобщението не се изпраща и забележите следното поведение:</span><span class="sxs-lookup"><span data-stu-id="232c2-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="232c2-109">За работен поток с помощта на SharePoint 2013 платформа тип преминете към страницата на **състоянието на работния поток** .</span><span class="sxs-lookup"><span data-stu-id="232c2-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="232c2-110">На страницата състояние на работния поток **вътрешно състояние** е настроен да **стартира**и информация балон показва **не може да изпрати на получател**.</span><span class="sxs-lookup"><span data-stu-id="232c2-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="232c2-111">За да заобиколите този проблем, конфигурирайте вашия работен поток за изпращане на имейл съобщения, без да надвишава [границите на Exchange Online подател](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="232c2-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="232c2-112">Например използвайте пауза в работния поток, изпращане на имейл до група на Office 365, група за разпространение или електронна поща разрешено група за защита, или изпращане на съобщението до по-малко от 200 получатели наведнъж.</span><span class="sxs-lookup"><span data-stu-id="232c2-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="232c2-113">За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="232c2-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="232c2-114">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="232c2-114">Related topics</span></span>
- [<span data-ttu-id="232c2-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="232c2-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="232c2-116">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="232c2-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 