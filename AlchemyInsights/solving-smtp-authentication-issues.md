---
title: Разрешаване на проблеми с SMTP удостоверяване
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264317"
---
# <a name="solving-smtp-authentication-issues"></a>Разрешаване на проблеми с SMTP удостоверяване

Ако получавате грешки 5.7.57 или 5.7.3, когато се опитвате да изпратите SMTP имейл и удостоверяване с клиент или приложение, има няколко неща, които трябва да проверите:

- Удостоверено изпращане на SMTP може да бъде забранено в клиента или в пощенската кутия, която се опитвате да използвате (проверете и двете настройки). За да прочетете повече, вижте [Разрешаване или забраняване на удостоверени клиент SMTP подаване](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Проверете дали [Azure сигурност по подразбиране](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) са разрешени за вашия клиент; ако е разрешено, SMTP удостоверяване с използване на базово удостоверяване (известно още като наследено; това ще използва потребителско име и парола) ще се провали.
