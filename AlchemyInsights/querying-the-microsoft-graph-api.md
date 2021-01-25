---
title: Заявка за Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974181"
---
# <a name="querying-the-microsoft-graph-api"></a>Заявка за Microsoft Graph API

Тази тема може да се приложи и за разработчиците, които все още използват Azure AD Graph API. Все пак **настоятелно** се препоръчва да използвате Microsoft Graph за всички сценарии на вашия указател, самоличност и управление на достъпа.

**Проблеми при удостоверяване или упълномощаване**

- Ако вашето приложение не е в **състояние да получи маркери** , за да се обадите на Microsoft Graph, изберете **проблем** , за да получите по-конкретна помощ и поддръжка на тази тема.
- Ако вашето приложение **получава грешки за удостоверяване на 401 или 403** , когато се обаждате на Microsoft Graph, изберете категорията API за **получаване на отказан достъп (разрешение)** Microsoft Graph, за да получите по-конкретна помощ и поддръжка на тази тема.

**Искам да използвам Microsoft Graph, но не знам откъде да започна**

За да научите повече за Microsoft Graph, вижте:

- [Общ преглед на Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор на управлението на самоличността и достъпа в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Първи стъпки в създаването на приложения на Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демонстрация

**Искам да използвам Microsoft Graph, но поддържа ли API за v 1,0 директорията, от която се нуждая?**

Microsoft Graph представлява препоръчвания API за адресна книга, самоличност и управление на достъпа. Но все още има някои пропуски между това, което е възможно в Azure AD Graph и Microsoft Graph. Прегледайте статиите по-долу, които осветяват най-актуалните разлики, за да ви помогнат по ваш избор:

- [Разлики между типовете ресурси между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Разлики между свойствата между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Разлики в методите между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Когато задавам заявка за *потребителския* обект, много от свойствата му липсват**

`GET https://graph.microsoft.com/v1.0/users` връща само 11 свойства, тъй като Microsoft Graph автоматично избира набор от *потребителски* свойства по подразбиране, за да се върне. Ако имате нужда от други *потребителски* свойства, използвайте $Select, за да изберете свойствата, от които се нуждае вашата заявка. Изпробвайте го първо в **Microsoft Graph Explorer** .

**Някои потребителски стойности на свойства са *NULL* въпреки че знам, че са зададени**

Най-вероятно обяснение е, че приложението е дало на *потребителя. ReadBasic. All* разрешение. Това позволява на приложението да прочете ограничен набор от потребителски свойства, като връща всички други свойства като Null дори ако са били предварително зададени. Опитайте да отпуснете приложението *User. read. All* разрешение вместо това.

За повече информация вижте [потребителски разрешения за Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Имам проблеми с използването на параметри на заявката OData за филтриране на данни в моите искания**

Докато Microsoft Graph поддържа широк диапазон от параметри на заявката за OData, много от тези параметри не се поддържат напълно от справочните услуги (ресурси, които се наследяват от *directoryObject*) в Microsoft Graph. Същите ограничения, които присъстваха в Azure AD Graph, продължават по-голямата част от Microsoft Graph:

1. **Не се поддържа**: $count, $search и $Filter върху стойности *NULL* или *NOT NULL*
2. **Не се поддържа**: $Filter за определени свойства (Вижте теми за ресурси, в които свойствата могат да се филтрират)
3. **Не се поддържа**: страниране, филтриране и сортиране едновременно
4. **Не се поддържа**: филтриране по релация. Например – Намерете всички членове на инженерната група, които са в Обединеното кралство.
5. **Частична поддръжка**: $orderby на *потребител* (само за displayName и userPrincipalName) и *Група*
6. **Частична поддръжка**: $Filter (поддържа само *EQ*, *startswith* *или*, *и* и ограничава *всякакви*) поддръжка $expand (разширяването на релациите на един обект връща всички релации, но разширяването на колекция от релации на обекти е ограничено)

За повече информация вижте [Персонализиране на отговори с параметри на заявка](https://docs.microsoft.com/graph/query-parameters).

**API-то, на което се обаждам, не работи – къде мога да направя още тестване?**

**Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демо и също така разгледайте **примерните заявки** в Microsoft Graph Explorer.

**Когато имам заявка за данни, изглежда, че получавам незавършен набор данни обратно**

Ако задавате заявка за събиране (като *потребители*), Microsoft Graph използва ограничения за страниците на сървъра, така че резултатите винаги да се връщат с размер на страницата по подразбиране. Приложението ви трябва винаги да очаква да се изпраща на страница чрез колекции, върнати от услугата.

За повече информация вижте:

- [Най-добри практики за Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Пейджинг данни за Microsoft Graph във вашето приложение](https://docs.microsoft.com/graph/paging)

**Приложението ми е твърде бавно и все още не може да се регулира. Какви подобрения мога да направя?**

В зависимост от сценария ви има редица различни опции на ваше разположение, за да направите приложението си по-съобразно и в някои случаи по-малко податливи на ограничаване на услугата (когато провеждате твърде много обаждания).

За да научите повече, вижте:

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
