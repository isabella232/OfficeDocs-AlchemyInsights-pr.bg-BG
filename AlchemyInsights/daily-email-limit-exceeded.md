---
title: Ограничението за дневен имейл е надвишено. Работният поток се отменя.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731552"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="17e21-103">Ограничението за дневен имейл е надвишено.</span><span class="sxs-lookup"><span data-stu-id="17e21-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="17e21-104">Работният поток се отменя.</span><span class="sxs-lookup"><span data-stu-id="17e21-104">Workflow is suspended.</span></span>

<span data-ttu-id="17e21-105">Тази грешка може да бъде получена в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="17e21-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="17e21-106">Имате работен поток в SharePoint Online, който използва типа на платформата за работен поток на SharePoint 2010 или SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="17e21-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="17e21-107">Работният поток е конфигуриран да изпраща имейл съобщение по избор до повече от потребители на 200 едновременно, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="17e21-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="17e21-108">Когато стартирате работния поток, имейл съобщението не се изпраща и забелязвате следното поведение:</span><span class="sxs-lookup"><span data-stu-id="17e21-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="17e21-109">За работен поток, използващ типа платформа на SharePoint 2013, трябва да отидете на страницата " **състояние на работния поток** ".</span><span class="sxs-lookup"><span data-stu-id="17e21-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="17e21-110">В страницата "състояние на работния поток" **вътрешното състояние** е зададено на " **стартиран**" и балонът с информация **не може да се изпрати до получателя**.</span><span class="sxs-lookup"><span data-stu-id="17e21-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="17e21-111">За да заобиколите този проблем, конфигурирайте своя работен поток, за да изпращате имейл съобщения, без да надвишавате [ограничението за подателя на Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="17e21-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="17e21-112">Например използвайте пауза в работния поток, изпратете имейла до група на Microsoft 365, група за разпространение или група за защита с активиран имейл или изпратете съобщението до по-малко от 200 получатели едновременно.</span><span class="sxs-lookup"><span data-stu-id="17e21-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="17e21-113">За повече информация вижте [статията](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)по-долу.</span><span class="sxs-lookup"><span data-stu-id="17e21-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="17e21-114">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="17e21-114">Related topics</span></span>
- [<span data-ttu-id="17e21-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="17e21-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="17e21-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="17e21-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 