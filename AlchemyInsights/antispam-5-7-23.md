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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932158"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Коригиране на проблеми с доставянето на имейл за код на грешка 5.7.23

Проверете SPF DNS записа за вашия домейн в публично достъпна проверка на SPF или DNS записи в уеб.

Уверете се, че изходящо съобщение не е идентифицирано като спам от Microsoft и маршрутизирани през набора за доставяне [с висок риск.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Съобщенията в набора с високорискови доставки няма да преминат SPF проверки и следователно няма да бъдат приети от организацията за имейл на местоназначението.

Ако проблемът продължава, може да се наложи да се обърнете към администратора на имейл хоста, на който се опитвате да изпратите имейл. Обърнете внимание на подробната външна грешка, налична в съобщението за отпадане. Поддръжката на Microsoft може да не успее да ви помогне допълнително.
