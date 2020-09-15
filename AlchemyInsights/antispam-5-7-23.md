---
title: Антиспам – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717314"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="57b91-102">Отстраняване на проблеми с доставянето на имейл за код на грешка 5.7.23</span><span class="sxs-lookup"><span data-stu-id="57b91-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="57b91-103">Проверете SPF DNS записа за вашия домейн в публично достъпна програма за проверка на SPF или DNS записи в уеб.</span><span class="sxs-lookup"><span data-stu-id="57b91-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="57b91-104">Проверете дали изходящо съобщение не е идентифицирано като нежелана поща от Microsoft и се маршрутизира през [басейна с висок риск за доставяне](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="57b91-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="57b91-105">Съобщения във високорисковия набор за доставяне на риск няма да премине SPF проверки и следователно няма да бъдат приети от имейл организацията местоназначение.</span><span class="sxs-lookup"><span data-stu-id="57b91-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="57b91-106">Ако проблемът продължава, може да се наложи да се обърнете към администратора на пощенския хост, към който се опитвате да изпратите имейл.</span><span class="sxs-lookup"><span data-stu-id="57b91-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="57b91-107">Напомнете подробни външни грешки, налични в прескачащо съобщение.</span><span class="sxs-lookup"><span data-stu-id="57b91-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="57b91-108">Поддръжката на Microsoft може да не е в състояние да помогне по-нататък.</span><span class="sxs-lookup"><span data-stu-id="57b91-108">Microsoft support may not be able to assist further.</span></span>
