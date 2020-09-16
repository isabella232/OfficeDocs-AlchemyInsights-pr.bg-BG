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
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="91e52-102">Решаване на проблеми с удостоверяването на SMTP</span><span class="sxs-lookup"><span data-stu-id="91e52-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="91e52-103">Ако получавате грешки 5.7.57 или 5.7.3, когато се опитвате да изпратите SMTP имейл и удостоверяване с клиент или приложение, има няколко неща, които трябва да проверите:</span><span class="sxs-lookup"><span data-stu-id="91e52-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="91e52-104">Автентичното предаване на SMTP може да е забранено за вашия клиент или за пощенската кутия, която се опитвате да използвате (Проверете и двете настройки).</span><span class="sxs-lookup"><span data-stu-id="91e52-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="91e52-105">За да прочетете повече, вижте [Разрешаване или забраняване на удостоверяване на автентично SMTP клиентско предаване](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="91e52-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="91e52-106">Проверете дали [настройките по подразбиране на Azure за защита](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) са разрешени за вашия клиент; Ако е разрешена, SMTP удостоверяване чрез основно удостоверяване (наричано още наследство; това ще използва потребителско име и парола) ще бъде неуспешно.</span><span class="sxs-lookup"><span data-stu-id="91e52-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
