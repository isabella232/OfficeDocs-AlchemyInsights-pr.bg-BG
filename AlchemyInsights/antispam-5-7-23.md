---
title: Антиспам – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821400"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f683e-102">Коригиране на проблеми с доставянето на имейл за код на грешка 5.7.23</span><span class="sxs-lookup"><span data-stu-id="f683e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f683e-103">Проверете SPF DNS записа за вашия домейн в публично достъпна проверка на SPF или DNS записи в уеб.</span><span class="sxs-lookup"><span data-stu-id="f683e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f683e-104">Уверете се, че изходящо съобщение не е идентифицирано като спам от Microsoft и маршрутизирани през набора за доставяне [с висок риск.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="f683e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f683e-105">Съобщенията в набора с високорискови доставки няма да преминат SPF проверки и следователно няма да бъдат приети от организацията за имейл на местоназначението.</span><span class="sxs-lookup"><span data-stu-id="f683e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f683e-106">Ако проблемът продължава, може да се наложи да се обърнете към администратора на имейл хоста, на който се опитвате да изпратите имейл.</span><span class="sxs-lookup"><span data-stu-id="f683e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f683e-107">Обърнете внимание на подробната външна грешка, налична в съобщението за отпадане.</span><span class="sxs-lookup"><span data-stu-id="f683e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f683e-108">Поддръжката на Microsoft може да не успее да ви помогне допълнително.</span><span class="sxs-lookup"><span data-stu-id="f683e-108">Microsoft support may not be able to assist further.</span></span>
