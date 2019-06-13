---
title: Запознаване с SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770552"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="c015b-102">Работни потоци в SharePoint</span><span class="sxs-lookup"><span data-stu-id="c015b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="c015b-103">Ако SharePoint потоци не изпращате имейли, вашата организация може да са срещали границите на Exchange Online подател.</span><span class="sxs-lookup"><span data-stu-id="c015b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="c015b-104">"Поток е спряно" съобщение за грешка може да възникне, ако имате един от следните елементи:</span><span class="sxs-lookup"><span data-stu-id="c015b-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="c015b-105">Имате работен поток в SharePoint Online, която използва SharePoint 2010 или SharePoint 2013 поток платформа тип.</span><span class="sxs-lookup"><span data-stu-id="c015b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="c015b-106">Работният поток е конфигуриран за изпращане на персонализирани имейл съобщение до повече от 200 потребители в даден момент, повече от 10000 получатели на ден или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="c015b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="c015b-107">Когато стартирате работния поток, имейл съобщението не е изпратено, и забележите съобщение за грешка, вътрешни състоянието е зададено се показва окачени или не може да изпрати на получател.</span><span class="sxs-lookup"><span data-stu-id="c015b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="c015b-108">За повече информация моля вижте следната [статия](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="c015b-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>
