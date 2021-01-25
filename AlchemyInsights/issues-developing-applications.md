---
title: Проблеми при разработване на приложения
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974188"
---
# <a name="issues-developing-applications"></a>Проблеми при разработване на приложения

За да отстраните най-често срещаните проблеми при създаването на приложения на Azure Active Directory (AD), вижте следните статии:

- [Виждам неприятности при влизане в приложения, които използват само браузъра Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Не знам как да променя настройките по подразбиране на токена за моето приложение](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Притеснен съм относно това как работи дадено съгласие за приложение](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Не знам как да давам разрешения за моето приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Не разбирам разликата между разрешения за делегиран и приложение](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за AZURE ad Graph (пад Graph)** _

- Започвайки от 30 юни 2020, повече няма да добавяме нови функции към библиотеката за удостоверяване на Azure Active Directory (ADAL) и API на Azure AD Graph (пад Graph). Ще продължим да предоставяме техническа поддръжка и актуализации на защитата, но повече няма да предоставяме актуализации на функции.

- Започвайки от 30 юни 2022, ние ще сложим край на поддръжката за ADAL и пад Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата. В резултат на това условие по-долу са посочени следните последствия:

    - Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма да получат техническа поддръжка или актуализация на защитата.

    - Приложенията, използващи пад Graph след този час, вече не могат да получават отговори от крайна точка на графиката с пад

_ *ADALна миграция**

Ако използвате приложения на Microsoft, ви препоръчваме да актуализирате до библиотеката за удостоверяване на Microsoft (MSAL), която има най-новите функции и актуализации на защитата. Тази препоръка е в контекста на Microsoft за започване на процеса на мигриране на приложенията към MSAL от крайния срок за поддръжка. 

Мигрирането от Microsoft на приложенията към MSAL гарантира, че приложенията се възползват от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Научете повече за това как да мигрирате приложения на база платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и, ако е приложимо, да се свържете с всички независими доставчици на софтуер (ISV) или доставчици на приложения. Поддръжката на Microsoft може да ви предостави и списък с всички приложения, които не са на Microsoft ADAL, във вашия клиент.

**Преминаване към графиката в пад**

За приложенията, които използват пад Graph, следвайте нашите указания за мигриране на приложения на "пад Graph" към Microsoft Graph:

1. [Нашият контролен списък за мигриране предоставя първи стъпки](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Вашият портал за регистрация на Azure App показва кои приложения използват пад Graph. Препоръчваме ви да прегледате всички изходни кодове на вашите приложения и, ако е приложимо, да се свържете с всички независими доставчици на софтуер (ISV) или с доставчиците на приложения. Поддръжката на Microsoft може да ви предостави и информация за използването на пад Graph във вашия клиент.







