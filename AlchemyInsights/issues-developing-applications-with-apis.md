---
title: Проблеми с разработването на приложения с API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013449"
---
# <a name="issues-developing-applications-with-apis"></a>Проблеми с разработването на приложения с API

За да започнете да използвате API Azure Active Directory Graph, вижте ръководството за бърз старт на [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) или прегледайте интерактивната документация за справка за Azure AD Graph [API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Край на поддръжката за Azure Active Directory удостоверяване (ADAL) и Azure AD Graph API (AAD Graph)**

**От 30 юни 2020 г.** вече няма да добавяме нови функции към ADAL и Azure AD Graph. Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

**От 30 юни 2022 г.** ще прекратим поддръжката за ADAL и Azure AD Graph и повече няма да предоставяме техническа поддръжка или актуализации на защитата.

Приложенията, които използват ADAL в съществуващи версии на операционната система, ще продължат да работят и след този момент, но няма да получават никаква техническа поддръжка и актуализации на защитата.

Приложенията, които използват Azure AD Graph след този период, може вече да не получават отговори от крайната точка на Azure AD Graph.

**Мигриране на ADAL**

Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.

Ако използвате приложенията на Microsoft, знайте, че Microsoft е в процес на мигриране на приложенията към MSAL до крайния срок за прекратяване на поддръжката, като гарантира, че те ще се възползват от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Научете как да мигрирате приложения на база платформа.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Ако имате нужда от помощ при разбирането кои от вашите приложения използват ADAL, ви препоръчваме да прегледате целия изходен код на вашите приложения и ако е приложимо, да се свържете с доставчиците на интернет услуги или приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложения, които използват Azure AD Graph, следвайте нашите указания, за да мигрирате [Azure AD Graph приложения към Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Нашият контролен списък за мигриране ви дава отправна точка](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения. Поддръжката от Microsoft може също да ви предостави списък с всички Graph на AAD във вашия клиент.
1. За да може вашето приложение да има достъп до данни Graph Microsoft, потребителят или администраторът трябва да му даде правилните разрешения чрез процес на съгласие. Препратката [към Graph разрешения на Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) показва разрешенията, свързани с всеки основен набор от API Graph Microsoft. Той също така предоставя указания как да използвате разрешенията.
