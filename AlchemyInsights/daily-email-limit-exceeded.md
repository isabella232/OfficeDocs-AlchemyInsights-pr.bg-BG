---
title: Ежедневно имейл граница превишавам. Работният поток е спряно.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514430"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="0fd46-103">Всекидневен email граница превишавам.</span><span class="sxs-lookup"><span data-stu-id="0fd46-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="0fd46-104">Работният поток е спряно.</span><span class="sxs-lookup"><span data-stu-id="0fd46-104">Workflow is suspended.</span></span>

<span data-ttu-id="0fd46-105">Тази грешка може да бъдат получени в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="0fd46-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="0fd46-106">Имате работен поток в SharePoint Online, която използва SharePoint 2010 или SharePoint 2013 поток платформа тип.</span><span class="sxs-lookup"><span data-stu-id="0fd46-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="0fd46-107">Работният поток е конфигуриран за изпращане на персонализирани имейл съобщение до повече от 200 потребители в даден момент, повече от 10000 получатели на ден или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="0fd46-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="0fd46-108">Когато стартирате работния поток, имейл съобщението не е изпратено, и забележите следното поведение:</span><span class="sxs-lookup"><span data-stu-id="0fd46-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="0fd46-109">За работен поток, като използвате SharePoint 2013 платформа тип преминете към страницата на **Състоянието на работния поток** .</span><span class="sxs-lookup"><span data-stu-id="0fd46-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="0fd46-110">В страницата състояние на работния поток **Вътрешно състояние** е настроено да **започнем**и балона с информация показва **не може да изпрати на получател**.</span><span class="sxs-lookup"><span data-stu-id="0fd46-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="0fd46-111">За да заобиколите този проблем, конфигурирайте вашия работен поток да изпрати имейл съобщения без превишаване на [Exchange Online подателя граници](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="0fd46-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="0fd46-112">Например използвайте пауза в работния поток, изпращане на имейл до Office 365 група, група за разпространение или група за защита на поща разрешени или изпращане на съобщение до по-малко от 200 получатели в даден момент.</span><span class="sxs-lookup"><span data-stu-id="0fd46-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="0fd46-113">За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="0fd46-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="0fd46-114">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="0fd46-114">Related topics</span></span>
- [<span data-ttu-id="0fd46-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="0fd46-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0fd46-116">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="0fd46-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 