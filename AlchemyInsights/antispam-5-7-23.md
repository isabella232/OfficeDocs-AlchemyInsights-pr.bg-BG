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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Отстраняване на проблеми с доставката на имейл за код на грешка 5.7.23

Проверете SPF DNS запис за вашия домейн в публично достъпни SPF или DNS запис за проверка в мрежата.

Уверете се, че изходящото съобщение не е било идентифицирано като спам от Office 365 и е пренасочено през [големия набор за доставка на риск](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Съобщения в басейна на високорисковите доставка няма да премине SPF проверки и следователно няма да бъдат приемани от местоназначението имейл организация.

Ако проблемът продължава, може да се наложи да се свържете с администратора на имейл хоста, към който се опитвате да изпратите имейл. Отбележете подробната външна грешка, налична в съобщението за отпадане.  Поддръжката на Office 365 може да не може да помогне повече.