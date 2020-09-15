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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Отстраняване на проблеми с доставянето на имейл за код на грешка 5.7.23

Проверете SPF DNS записа за вашия домейн в публично достъпна програма за проверка на SPF или DNS записи в уеб.

Проверете дали изходящо съобщение не е идентифицирано като нежелана поща от Microsoft и се маршрутизира през [басейна с висок риск за доставяне](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Съобщения във високорисковия набор за доставяне на риск няма да премине SPF проверки и следователно няма да бъдат приети от имейл организацията местоназначение.

Ако проблемът продължава, може да се наложи да се обърнете към администратора на пощенския хост, към който се опитвате да изпратите имейл. Напомнете подробни външни грешки, налични в прескачащо съобщение. Поддръжката на Microsoft може да не е в състояние да помогне по-нататък.
