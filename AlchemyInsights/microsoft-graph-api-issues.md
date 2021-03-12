---
title: Проблеми с API на Microsoft Graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713360"
---
# <a name="microsoft-graph-api-issues"></a>Проблеми с API на Microsoft Graph

Тази тема може да се приложи и за разработчиците, които все още използват Azure AD Graph API. Все пак **настоятелно** се препоръчва да използвате Microsoft Graph за всички сценарии на вашия указател, самоличност и управление на достъпа.

**Проблеми при удостоверяване или упълномощаване**

- Ако вашето приложение не е в **състояние да получи маркери** , за да се обадите на Microsoft Graph, изберете **проблем** , за да получите по-конкретна помощ и поддръжка на тази тема.
- Ако вашето приложение **получава грешки за удостоверяване на 401 или 403** , когато се обаждате на Microsoft Graph, изберете категорията API за **получаване на отказан достъп (разрешение)** Microsoft Graph, за да получите по-конкретна помощ и поддръжка на тази тема.

**Искам да използвам Microsoft Graph, но не знам откъде да започна**

- [Общ преглед на Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор на управлението на самоличността и достъпа в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Първи стъпки в създаването на приложения на Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демонстрация

**Искам да използвам Microsoft Graph, но поддържа ли API за v 1,0 директорията, от която се нуждая?**

Microsoft Graph представлява препоръчвания API за адресна книга, самоличност и управление на достъпа. Но все още има някои пропуски между това, което е възможно в Azure AD Graph и Microsoft Graph. Прегледайте статиите по-долу, които осветяват най-актуалните разлики, за да ви помогнат по ваш избор:

- [Разлики между типовете ресурси между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Разлики между свойствата между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Разлики в методите между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API за обаждане не работи – къде мога да направя още тестване?**

**Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демо и също така разгледайте **примерните заявки** в Microsoft Graph Explorer.

**Приложението ми е твърде бавно и все още не може да се регулира. Какви подобрения мога да направя?**

В зависимост от сценария ви има редица опции, с които разполагате, за да направите приложението си по-съобразно и в някои случаи по-малко податливи на ограничаване на услугата (когато провеждате твърде много обаждания).

- [Най-добри практики за Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Изисквания за дозиране](https://docs.microsoft.com/graph/json-batching)
- [Следене на промените чрез Делта заявка](https://docs.microsoft.com/graph/delta-query-overview)
- [Получаване на известие за промените чрез webhooks](https://docs.microsoft.com/graph/webhooks)
- [Ограничаване на указания](https://docs.microsoft.com/graph/throttling)

**Къде мога да намеря повече информация за грешки и известни проблеми?**

- [Информация за отговора на грешката на Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Известни проблеми с Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Къде мога да проверя състоянието на наличност и свързване на услугата?**

Наличността на услугата и свързването на основните услуги, които са достъпни чрез Microsoft Graph, могат да окажат влияние върху цялостната достъпност и производителност на Microsoft Graph.

- За изправност на услугата Azure Active Directory Проверете състоянието на услугите за **защита + самоличност** , показани в [страницата за състояние на Azure](https://azure.microsoft.com/status/).
- За услуги на Office, които допринасят за Microsoft Graph, проверете състоянието на услугите, които са посочени в [таблото за изправност на услугите на Office](https://portal.office.com/adminportal/home#/servicehealth).

Грешките при удостоверяване на Microsoft Graph могат да се дължат на няколко различни проблема, като повечето от тях генерират грешка 401 или 403. Например следното може да доведе до грешки при удостоверяване:

- Неправилни [потоци на придобиване на маркери за достъп](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неправилно конфигурирани [обхвати на разрешения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Липса на [съгласие](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и Azure AD Graph API (AAD Graph)_* _

_ * Започване на 30 юни 2020 * *, повече няма да добавяме нови функции към ADAL и Azure AD Graph. Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.

**Започвайки от 30 юни 2022**, ние ще прекратим ПОДДРЪЖКАТА за ADAL и Azure ad Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.

Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма *да получат техническа поддръжка или актуализация на защитата*.

Приложенията, използващи Azure AD Graph след този час, вече не могат да получават отговори от крайна точка на Azure AD Graph.

**ADALна миграция**

Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.

Ако използвате Microsoft Apps, Знайте, че Microsoft е в процес на мигриране на приложенията си към MSAL до крайния срок за поддръжка, за да се гарантира, че ще извлече полза от текущите подобрения в защитата и функциите на MSAL.

1. [Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Научете как да мигрирате приложения на базата на платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и ако е приложимо, да достигнете до всякакви доставчици на ISV или приложения. Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.

**Мигриране на AAD Graph**

За приложенията, които използват Azure AD Graph, следвайте нашите указания за [мигриране на приложенията на AZURE ad Graph към Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Нашият контролен списък за мигриране ви дава отправна точка](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph. Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения. Поддръжката на Microsoft може да ви предостави и списък на всички употреби на използването на пад във вашия клиент.
3. За да получите достъп до данните в Microsoft Graph, потребителят или администраторът трябва да му предостави правилните разрешения чрез процеса на одобрение. [Справочникът за разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) изброява разрешенията, свързани с всеки основен набор от API на Microsoft Graph. Освен това се предоставят насоки как да използвате разрешенията.
