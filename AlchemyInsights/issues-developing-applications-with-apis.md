---
title: Проблеми при разработване на приложения с API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974264"
---
# <a name="issues-developing-applications-with-apis"></a>Проблеми при разработване на приложения с API

За да започнете да използвате API на Azure Active Directory, вижте [справочника за ръководство за бърз старт в AZURE ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) или вижте [документацията за справочника за API за интерактивна Azure ad Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за Azure AD Graph (пад Graph)**

**Започвайки от 30 юни 2020**, повече няма да добавяме нови функции към ADAL и Azure ad Graph. Ще продължим да предоставяме техническа поддръжка и актуализации на защитата, но повече няма да предоставяме актуализации на функции.

**Започвайки от 30 юни 2022**, ние ще прекратим ПОДДРЪЖКАТА за ADAL и Azure ad Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.

Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма да получат техническа поддръжка или актуализация на защитата.

Приложенията, използващи Azure AD Graph след този час, вече не могат да получават отговори от крайна точка на Azure AD Graph.

**ADALна миграция**

Препоръчваме ви да актуализирате до [библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), която има най-новите функции и актуализации на защитата.

Ако използвате Microsoft Apps, Знайте, че Microsoft е в процес на мигриране на приложенията си към MSAL до крайния срок за поддръжка, за да се гарантира, че ще извлече полза от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Научете как да мигрирате приложения на база платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и ако е приложимо, да достигнете до всякакви доставчици на ISV или приложения. Поддръжката на Microsoft може да ви предостави и списък с всички приложения, които не са на Microsoft ADAL, във вашия клиент.

**Преминаване към графиката в пад**

За приложенията, които използват Azure AD Graph, следвайте нашите указания за мигриране на [приложенията на AZURE ad Graph към Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Нашият контролен списък за мигриране предоставя първи стъпки](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Вашият портал за регистрация на Azure App показва кои приложения използват пад Graph. Препоръчваме ви да прегледате всички изходни кодове на вашите приложения и ако е приложимо, да се свържете с всички доставчици на ISV или приложения. Поддръжката на Microsoft може да ви предостави и списък на всички употреби на използването на пад във вашия клиент.
1. За да получите достъп до данните в Microsoft Graph, потребителят или администраторът трябва да му предостави правилните разрешения чрез процеса на одобрение. [Справочникът за разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) изброява разрешенията, свързани с всеки основен набор от API на Microsoft Graph. Освен това се предоставят насоки как да използвате разрешенията.
