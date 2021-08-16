---
title: Проблеми с библиотеките за удостоверяване
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027993"
---
# <a name="issues-with-authentication-libraries"></a>Проблеми с библиотеките за удостоверяване

1. [Платформа за самоличност на Microsoft за удостоверяване изброява](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) поддържани от Microsoft и съвместими библиотеки с клиенти и мидълуер.
2. Библиотеката за удостоверяване на Microsoft (MSAL) поддържа няколко [потока на удостоверяване](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) за използване в различни сценарии на приложения.
3. За да удостоверите и придобиете маркери, вие инициализирате ново публично или поверително клиентско приложение във вашия код. Можете да зададете няколко опции за конфигуриране, когато инициализирате клиентското приложение в библиотеката за удостоверяване на Microsoft (MSAL). За да научите повече, вижте Опции [за конфигуриране на приложението](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Край на поддръжката за Azure Active Directory удостоверяване (ADAL) и Azure AD Graph API (AAD Graph)**

**От 30 юни 2020 г.** вече няма да добавяме нови функции към ADAL и Azure AD Graph. Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

**От 30 юни 2022 г.** ще прекратим поддръжката за ADAL и Azure AD Graph и повече няма да предоставяме техническа поддръжка или актуализации на защитата.

Приложенията, които използват ADAL на съществуващи версии на операционната система, ще продължат да работят след този период, но няма да имат *никаква техническа поддръжка или актуализации на защитата.*

Приложенията, които използват Azure AD Graph след този период, може вече да не получават отговори от крайната точка на Azure AD Graph.

**Мигриране на ADAL**

Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.

Ако използвате приложения на Microsoft, знайте, че Microsoft е в процес на мигриране на неговите приложения към MSAL до крайния срок за прекратяване на поддръжката, като гарантира, че те ще се възползват от текущите подобрения в защитата и функциите на MSAL.

За повече информация вижте:

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Научете как да мигрирате приложения на базата на платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ако имате нужда от помощ при разбирането кои от вашите приложения използват ADAL, ви препоръчваме да прегледате целия изходен код на вашите приложения и ако е приложимо, да се свържете с доставчиците на интернет услуги или приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложения, които използват Azure AD Graph, следвайте нашите указания, за да мигрирате [Azure AD Graph приложения към Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Нашият контролен списък за мигриране предоставя отправна точка за първи стъпки.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения. Поддръжката от Microsoft може също да ви предостави списък с всички Graph на AAD във вашия клиент.
3. За да може вашето приложение да има достъп до данни Graph Microsoft, потребителят или администраторът трябва да му даде правилните разрешения чрез процес на съгласие. Препратката [към Graph разрешения на Microsoft](https://docs.microsoft.com/graph/permissions-reference) показва разрешенията, свързани с всеки основен набор от API Graph Microsoft. Той също така предоставя указания как да използвате разрешенията.
