---
title: Проблеми с API Graph microsoft Graph microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975882"
---
# <a name="microsoft-graph-api-issues"></a>Проблеми с API Graph microsoft Graph microsoft

Тази тема може да се отнася и за разработчици, които все още използват Azure AD Graph API. Настоятелно се препоръчва обаче **да използвате** Microsoft Graph за всички сценарии за управление на справочника, самоличността и достъпа.

**Проблеми с удостоверяването или удостоверяването**

- Ако приложението ви **не** може да придобие маркери, за да се обади на Microsoft Graph, изберете Проблем с получаването на маркер за достъп **(удостоверяване)** категория на Microsoft Graph, за да получите по-конкретна помощ и поддръжка по тази тема.
- Ако приложението ви получава **401 или 403** грешки при удостоверяване, когато се обажда на Microsoft Graph, изберете категорията Получаване на грешка отказан достъп **(удостоверяване)** на Microsoft Graph API, за да получите по-конкретна помощ и поддръжка по тази тема.

**Искам да използвам Microsoft Graph, но не съм сигурен откъде да започна**

- [Общ преглед на microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Общ преглед на управлението на самоличност и достъп в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Първи стъпки в изграждането на приложения Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – тествайте API Graph microsoft във вашия клиент или демонстрационен клиент

**Искам да използвам Microsoft Graph, но поддържа ли API на указателя v1.0, които ми трябват?**

Microsoft Graph е препоръчителният API за управление на справочника, самоличност и достъп. Въпреки това все още има няколко празнини между това, което е възможно в Azure AD Graph и Microsoft Graph. Прегледайте следните статии, които подчертават най-актуалните разлики, които да ви помогнат да изберете:

- [Разлики в типа на ресурсите между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Разлики в свойството между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Разлики в метода между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, на който се обаждам, не работи – къде мога да направя повече тестове?**

**Microsoft Graph Explorer** – тествайте API Graph microsoft във вашия клиент или демонстрационен клиент, а също и прегледайте **примерните** заявки в Microsoft Graph Explorer.

**Приложението ми е твърде бавно и също се затладява. Какви подобрения мога да направя?**

В зависимост от вашия сценарий, има различни опции, с които разполагате, за да направите приложението по-изпълнително, а в някои случаи по-малко склонни към ограничаване от услугата (когато провеждате твърде много повиквания).

- [Най-Graph практики на Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Заявки за партиди](https://docs.microsoft.com/graph/json-batching)
- [Проследяване на промените чрез делта заявка](https://docs.microsoft.com/graph/delta-query-overview)
- [Получаване на известие за промени чрез уеб шлюзове](https://docs.microsoft.com/graph/webhooks)
- [Указания за ограничаване](https://docs.microsoft.com/graph/throttling)

**Къде мога да намеря повече информация за грешки и известни проблеми?**

- [Microsoft Graph за отговор на грешка](https://docs.microsoft.com/graph/errors)
- [Известни проблеми с Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Къде мога да проверя състоянието на наличността и свързването на услугата?**

Наличността и свързаността на услугите, до които се осъществява достъп чрез Microsoft Graph, могат да влияят върху цялостната наличност и производителност на Microsoft Graph.

- За Azure Active Directory на услугата проверете състоянието на услугите **за защита + самоличност,** изброени на страницата [Състояние на Azure](https://azure.microsoft.com/status/).
- За Office, които допринасят за Microsoft Graph, проверете състоянието на услугите, изброени [в таблото Office из изздрави услугата](https://portal.office.com/adminportal/home#/servicehealth).

Грешките Graph удостоверяване на Microsoft могат да бъдат резултат от няколко различни проблема, повечето от които генерират грешка 401 или 403. Например всички по-долу могат да доведат до грешки при удостоверяване:

- Неправилни [потоци на придобиване на маркери за достъп](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неправилно конфигурирани [обхвати на разрешения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Липса на [съгласие](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Край на поддръжката за Azure Active Directory удостоверяване (ADAL) и Azure AD Graph API (AAD Graph)***

**От 30 юни 2020 г.** вече няма да добавяме нови функции към ADAL и Azure AD Graph. Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

**От 30 юни 2022 г.** ще прекратим поддръжката за ADAL и Azure AD Graph и повече няма да предоставяме техническа поддръжка или актуализации на защитата.

Приложенията, които използват ADAL на съществуващи версии на операционната система, ще продължат да работят след този период, но няма да имат *никаква техническа поддръжка или актуализации на защитата.*

Приложенията, които използват Azure AD Graph след този период, може вече да не получават отговори от крайната точка на Azure AD Graph.

**Мигриране на ADAL**

Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.

Ако използвате приложения на Microsoft, знайте, че Microsoft е в процес на мигриране на неговите приложения към MSAL до крайния срок за прекратяване на поддръжката, като гарантира, че те ще се възползват от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Научете как да мигрирате приложения на базата на платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ако имате нужда от помощ при разбирането кои от вашите приложения използват ADAL, ви препоръчваме да прегледате целия изходен код на вашите приложения и ако е приложимо, да се свържете с доставчиците на интернет услуги или приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложения, които използват Azure AD Graph, следвайте нашите указания, за да мигрирате [Azure AD Graph приложения към Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Нашият контролен списък за мигриране ви дава отправна точка](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения. Поддръжката от Microsoft може също да ви предостави списък с всички Graph на AAD във вашия клиент.
3. За да може вашето приложение да има достъп до данни Graph Microsoft, потребителят или администраторът трябва да му даде правилните разрешения чрез процес на съгласие. Препратката [към Graph разрешения на Microsoft](https://docs.microsoft.com/graph/permissions-reference) показва разрешенията, свързани с всеки основен набор от API Graph Microsoft. Той също така предоставя указания как да използвате разрешенията.
