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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063580"
---
# <a name="issues-with-authentication-libraries"></a>Проблеми с библиотеките за удостоверяване

1. [Библиотеките за удостоверяване на Microsoft Identity platforms](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) изброява поддържани и съвместими с Microsoft библиотеки клиент и междинен източник.
2. Библиотеката за удостоверяване на Microsoft (MSAL) поддържа няколко [потока на удостоверяване](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) за използване в различни сценарии за приложения.
3. За удостоверяване и получаване на маркери можете да инициализирате ново публично или поверително клиентско приложение в своя код. Можете да зададете няколко опции за конфигуриране, когато инициализирате приложението клиент в библиотеката за удостоверяване на Microsoft (MSAL). За да научите повече, вижте [Опции за конфигуриране на приложения](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за Azure AD Graph (пад Graph)**

**Започвайки от 30 юни 2020**, повече няма да добавяме нови функции към ADAL и Azure ad Graph. Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

**Започвайки от 30 юни 2022**, ние ще прекратим ПОДДРЪЖКАТА за ADAL и Azure ad Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.

Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма *да получат техническа поддръжка или актуализация на защитата*.

Приложенията, използващи Azure AD Graph след този час, вече не могат да получават отговори от крайна точка на Azure AD Graph.

**ADALна миграция**

Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.

Ако използвате Microsoft Apps, Знайте, че Microsoft е в процес на мигриране на приложенията си към MSAL до крайния срок за поддръжка, за да се гарантира, че ще извлече полза от текущите подобрения в защитата и функциите на MSAL.

За повече информация вижте:

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Научете как да мигрирате приложения на базата на платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и ако е приложимо, да достигнете до всякакви доставчици на ISV или приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложенията, които използват Azure AD Graph, следвайте нашите указания за [мигриране на приложенията на AZURE ad Graph към Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Нашият контролен списък за мигриране предоставя първи стъпки.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения. Поддръжката на Microsoft може да ви предостави и списък на всички употреби на използването на пад във вашия клиент.
3. За да получите достъп до данните в Microsoft Graph, потребителят или администраторът трябва да му предостави правилните разрешения чрез процеса на одобрение. [Справочникът за разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) изброява разрешенията, свързани с всеки основен набор от API на Microsoft Graph. Освен това се предоставят насоки как да използвате разрешенията.
