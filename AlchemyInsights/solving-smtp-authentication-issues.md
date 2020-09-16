---
title: Решаване на проблеми с удостоверяването на SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737978"
---
# <a name="solving-smtp-authentication-issues"></a>Решаване на проблеми с удостоверяването на SMTP

Ако получавате грешки 5.7.57 или 5.7.3, когато се опитвате да изпратите SMTP имейл и удостоверяване с клиент или приложение, има няколко неща, които трябва да проверите:

- Автентичното предаване на SMTP може да е забранено за вашия клиент или за пощенската кутия, която се опитвате да използвате (Проверете и двете настройки). За да прочетете повече, вижте [Разрешаване или забраняване на удостоверяване на автентично SMTP клиентско предаване](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Проверете дали [настройките по подразбиране на Azure за защита](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) са разрешени за вашия клиент; Ако е разрешена, SMTP удостоверяване чрез основно удостоверяване (наричано още наследство; това ще използва потребителско име и парола) ще бъде неуспешно.
