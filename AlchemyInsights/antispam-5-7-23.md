---
title: Антиспам - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676486"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="7380c-102">Отстраняване на проблеми с доставката на имейл за код на грешка 5.7.23</span><span class="sxs-lookup"><span data-stu-id="7380c-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="7380c-103">Проверете SPF DNS записа за вашия домейн на публично достъпна SPF или DNS проверка на записи в интернет.</span><span class="sxs-lookup"><span data-stu-id="7380c-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="7380c-104">Уверете се, че изходящото съобщение не е идентифицирано като спам от Microsoft и пренасочени през [високорисков доставка набор](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="7380c-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="7380c-105">Съобщенията в групата за високорискови доставки няма да преминат SPF проверки и следователно няма да бъдат приети от организацията местоназначение имейл.</span><span class="sxs-lookup"><span data-stu-id="7380c-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="7380c-106">Ако проблемът продължава, може да се наложи да се свържете с администратора на хоста за поща, на който се опитвате да изпратите имейл.</span><span class="sxs-lookup"><span data-stu-id="7380c-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="7380c-107">Обърнете внимание на подробната външна грешка, налична в съобщението за отпадане.</span><span class="sxs-lookup"><span data-stu-id="7380c-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="7380c-108">Поддръжката на Microsoft може да не е в състояние да помогне допълнително.</span><span class="sxs-lookup"><span data-stu-id="7380c-108">Microsoft support may not be able to assist further.</span></span>
