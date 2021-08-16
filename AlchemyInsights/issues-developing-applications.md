---
title: Проблеми с разработването на приложения
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013413"
---
# <a name="issues-developing-applications"></a>Проблеми с разработването на приложения

За отстраняване на най-често срещаните проблеми при Azure Active Directory приложения (AD), вижте следните статии:

- [Виждам проблеми с влизането в приложения само с помощта на браузъра Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Не знам как да променя настройките по подразбиране за живота на маркера за моето приложение](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Аз съм объркан за това как работи съгласието на приложението](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Не знам как да предоставя разрешения на моето приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Не разбирам разликата между делегирани и разрешения за приложение](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Край на поддръжката за Azure Active Directory удостоверяване (ADAL) и Azure AD Graph API (AAD Graph)***

- От 30 юни 2020 г. вече няма да добавяме нови функции към библиотеката за удостоверяване на Azure Active Directory (ADAL) и Azure AD Graph API (AAD Graph). Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

- От 30 юни 2022 г. ще прекратим поддръжката за ADAL и AAD Graph и повече няма да предоставяме актуализации на техническата поддръжка и защитата. В резултат на това условие последствията са следните:

    - Приложенията, които използват ADAL в съществуващи версии на операционната система, ще продължат да работят и след този момент, но няма да получават никаква техническа поддръжка и актуализации на защитата.

    - Приложенията, които използват AAD Graph след това време, може вече да не получават отговори от крайната точка на Graph AAD

**Мигриране на ADAL**

Ако използвате приложения на Microsoft, ви препоръчваме да актуализирате до библиотеката за удостоверяване на Microsoft (MSAL), която има най-новите функции и актуализации на защитата. Тази препоръка е в контекста на Microsoft, иницииращ процеса на мигриране на приложенията към MSAL до крайния срок за прекратяване на поддръжката. 

Мигрирането от Microsoft на неговите приложения към MSAL гарантира, че приложенията се възползват от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Научете как да мигрирате приложения на базата на платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ако имате нужда от помощ за разбиране кои от вашите приложения използват ADAL, ви препоръчваме да прегледате целия изходен код на вашите приложения и, ако е приложимо, да се свържете с независими доставчици на софтуер (ISVs) или доставчици на приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложения, които използват AAD Graph, следвайте нашите указания, за да мигрирате AAD Graph приложения към Microsoft Graph:

1. [Нашият контролен списък за мигриране ви дава отправна точка](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате целия изходен код на вашите приложения и, ако е приложимо, да се свържете с независими доставчици на софтуер (ISVs) или доставчици на приложения. Поддръжката на Microsoft може също да ви предостави информация за използването Graph AAD във вашия клиент.







