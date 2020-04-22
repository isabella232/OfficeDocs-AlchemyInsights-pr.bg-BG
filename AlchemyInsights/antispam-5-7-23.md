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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Отстраняване на проблеми с доставката на имейл за код на грешка 5.7.23

Проверете SPF DNS записа за вашия домейн на публично достъпна SPF или DNS проверка на записи в интернет.

Уверете се, че изходящото съобщение не е идентифицирано като спам от Microsoft и пренасочени през [високорисков доставка набор](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Съобщенията в групата за високорискови доставки няма да преминат SPF проверки и следователно няма да бъдат приети от организацията местоназначение имейл.

Ако проблемът продължава, може да се наложи да се свържете с администратора на хоста за поща, на който се опитвате да изпратите имейл. Обърнете внимание на подробната външна грешка, налична в съобщението за отпадане. Поддръжката на Microsoft може да не е в състояние да помогне допълнително.
