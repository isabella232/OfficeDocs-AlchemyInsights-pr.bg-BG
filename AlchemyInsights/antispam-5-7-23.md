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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506432"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Коригирайте проблемите с доставката на имейл за код на грешка 5.7.23

Проверете SPF DNS записа за вашия домейн в публично достъпни SPF или DNS рекордьор в интернет.

Проверете дали изходящото съобщение не е идентифицирано като спам от Microsoft и се насочва чрез [набора за високорискови доставки](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Съобщенията в набора за висока риск доставка няма да премине SPF проверки и затова няма да бъдат приети от имейл организацията местоназначение.

Ако проблемът продължава, може да се наложи да се свържете с администратора на хоста на поща, към който се опитвате да изпратите имейл. Обърнете внимание на подробната външна грешка, налична в съобщението за отпадане. Поддръжката на Microsoft може да не е в състояние да помогне допълнително.
