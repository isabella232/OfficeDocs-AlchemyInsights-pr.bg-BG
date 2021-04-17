---
title: Решаване на проблеми с SMTP удостоверяването
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826404"
---
# <a name="solving-smtp-authentication-issues"></a>Решаване на проблеми с SMTP удостоверяването

Ако получавате грешки 5.7.57 или 5.7.3, когато се опитвате да изпратите SMTP имейл и да удостоверите с клиент или приложение, има няколко неща, които трябва да проверите:

- Удостоверено SMTP подаване може да е забранено във вашия клиент или в пощенската кутия, която се опитвате да използвате (проверете и двете настройки). За да прочетете повече, вижте [Разрешаване или забраняване на удостоверено изпращане на SMTP клиент](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Проверете дали [azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) са разрешени за вашия клиент; ако е разрешено, SMTP удостоверяването чрез базово удостоверяване (известно още като наследено; това ще използва потребителско име и парола) ще бъде неуспешно.
