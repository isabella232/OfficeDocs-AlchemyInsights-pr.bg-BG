---
title: Антиспам-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682036"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="644dd-102">Отстраняване на проблеми с доставката на имейл за код на грешка 5.7.23</span><span class="sxs-lookup"><span data-stu-id="644dd-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="644dd-103">Проверете SPF DNS запис за вашия домейн в публично достъпни SPF или DNS запис за проверка в мрежата.</span><span class="sxs-lookup"><span data-stu-id="644dd-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="644dd-104">Уверете се, че изходящото съобщение не е било идентифицирано като спам от Office 365 и е пренасочено през [големия набор за доставка на риск](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="644dd-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="644dd-105">Съобщения в басейна на високорисковите доставка няма да премине SPF проверки и следователно няма да бъдат приемани от местоназначението имейл организация.</span><span class="sxs-lookup"><span data-stu-id="644dd-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="644dd-106">Ако проблемът продължава, може да се наложи да се свържете с администратора на имейл хоста, към който се опитвате да изпратите имейл.</span><span class="sxs-lookup"><span data-stu-id="644dd-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="644dd-107">Отбележете подробната външна грешка, налична в съобщението за отпадане.</span><span class="sxs-lookup"><span data-stu-id="644dd-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="644dd-108">Поддръжката на Office 365 може да не може да помогне повече.</span><span class="sxs-lookup"><span data-stu-id="644dd-108">Office 365 support may not be able to assist further.</span></span>