---
title: Първи стъпки в SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700696"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="389e7-102">Работни потоци в SharePoint</span><span class="sxs-lookup"><span data-stu-id="389e7-102">Workflows in SharePoint</span></span>

<span data-ttu-id="389e7-103">Ако в работните потоци на SharePoint не се изпращат имейли, вашата организация може да е срещнала ограничението за подателя на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="389e7-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="389e7-104">Съобщение за грешка "работният поток е временно прекратен", ако имате един от следните елементи:</span><span class="sxs-lookup"><span data-stu-id="389e7-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="389e7-105">Имате работен поток в SharePoint Online, който използва типа на платформата за работен поток на SharePoint 2010 или SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="389e7-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="389e7-106">Работният поток е конфигуриран да изпраща имейл съобщение по избор до повече от потребители на 200 едновременно, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.</span><span class="sxs-lookup"><span data-stu-id="389e7-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="389e7-107">Когато стартирате работния поток, имейл съобщението не се изпраща и забелязвате съобщението за грешка, вътрешно състояние е зададено като прекратено или не може да се изпрати на получателя.</span><span class="sxs-lookup"><span data-stu-id="389e7-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="389e7-108">За повече информация вижте [статията](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)по-долу.</span><span class="sxs-lookup"><span data-stu-id="389e7-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

