---
title: Запознаване с SharePoint online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766880"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="c452e-102">Работни потоци в SharePoint</span><span class="sxs-lookup"><span data-stu-id="c452e-102">Workflows in SharePoint</span></span>

<span data-ttu-id="c452e-103">Ако SharePoint работни потоци не изпращат имейли, вашата организация може да се натъкна на Exchange Online подател лимити.</span><span class="sxs-lookup"><span data-stu-id="c452e-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="c452e-104">Съобщение за грешка "работният поток е спряно" може да възникне, ако имате един от следните елементи:</span><span class="sxs-lookup"><span data-stu-id="c452e-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="c452e-105">Имате работен поток в SharePoint Online, използващ SharePoint 2010 или SharePoint 2013 работен поток платформа тип.</span><span class="sxs-lookup"><span data-stu-id="c452e-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="c452e-106">Работният поток е конфигуриран да изпраща потребителски имейл съобщение до повече от 200 потребители наведнъж, повече от 10 000 получатели на ден, или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="c452e-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="c452e-107">Когато стартирате работния поток, имейл съобщението не се изпраща и забележите съобщение за грешка, Вътрешен статус е спряно или не може да изпрати до получател се показва.</span><span class="sxs-lookup"><span data-stu-id="c452e-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="c452e-108">За повече информация, моля, вижте следната [статия](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="c452e-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

