---
title: Заявка за API на Microsoft Graph microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923228"
---
# <a name="querying-the-microsoft-graph-api"></a>Заявка за API на Microsoft Graph microsoft

Тази тема може да се отнася и за разработчици, които все още използват Azure AD Graph API. Настоятелно се препоръчва обаче **да използвате** Microsoft Graph за всички сценарии за управление на справочника, самоличността и достъпа.

**Проблеми с удостоверяването или удостоверяването**

- Ако приложението ви **не** може да придобие маркери, за да се обади на Microsoft Graph, изберете Проблем с получаването на маркер за достъп **(удостоверяване)** категория на Microsoft Graph, за да получите по-конкретна помощ и поддръжка по тази тема.
- Ако приложението ви получава **401 или 403** грешки при удостоверяване, когато се обажда на Microsoft Graph, изберете категорията Получаване на грешка отказан достъп **(удостоверяване)** на Microsoft Graph API, за да получите по-конкретна помощ и поддръжка по тази тема.

**Искам да използвам Microsoft Graph, но не съм сигурен откъде да започна**

За да научите повече за Microsoft Graph, вижте:

- [Общ преглед на microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Общ преглед на управлението на самоличност и достъп в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Първи стъпки в изграждането на приложения Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – тествайте API Graph microsoft във вашия клиент или демонстрационен клиент

**Искам да използвам Microsoft Graph, но поддържа ли API на указателя v1.0, които ми трябват?**

Microsoft Graph е препоръчителният API за управление на справочника, самоличност и достъп. Въпреки това все още има няколко празнини между това, което е възможно в Azure AD Graph и Microsoft Graph. Прегледайте следните статии, които подчертават най-актуалните разлики, които да ви помогнат да изберете:

- [Разлики в типа на ресурсите между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Разлики в свойството между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Разлики в метода между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Когато заящам *потребителския* обект, много от свойствата му липсват**

`GET https://graph.microsoft.com/v1.0/users`връща само 11 свойства, тъй като Microsoft Graph автоматично избира набор от потребителски свойства по подразбиране *за* връщане. Ако имате нужда от *други потребителски* свойства, използвайте $select, за да изберете свойствата, от които се нуждае вашето приложение. Изпробвайте първо в **Microsoft Graph Explorer.**

**Някои стойности на потребителските свойство *са null,* въпреки че знам, че са зададени**

Най-вероятното обяснение е, че на приложението е дадено *разрешение User.ReadBasic.All.* Това позволява на приложението да прочете ограничен набор от потребителски свойства, връщайки всички други свойства като null дори ако преди това са били зададени. Опитайте да дадете разрешение *на приложението User.Read.All* вместо това.

За повече информация вижте [Разрешения на Graph microsoft](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Имам проблеми с използването на параметри на заявки на OData за филтриране на данни в моите заявки**

Въпреки че Microsoft Graph поддържа широк диапазон от параметрите на заявката OData, много от тези параметри не се поддържат напълно от справочните услуги (ресурси, които се наследяват от *справочникаObject*) в Microsoft Graph. Същите ограничения, които са били налични в Azure AD, Graph продължават в по-голямата си част в Microsoft Graph:

1. **Не се поддържа**: $count, $search и $filter стойности *null* или *не null*
2. **Не се поддържа:**$filter определени свойства (вж. темите за ресурси, на които свойствата могат да се филтрират)
3. **Не се поддържа**: едновременно страниране, филтриране и сортиране
4. **Не се поддържа:** филтриране на релация. Например – намерете всички членове на инженерната група, които са в Обединеното кралство.
5. **Частична** поддръжка : $orderby *на потребител* (само за displayName и userPrincipalName) и *група*
6. **Частична** поддръжка: $filter (поддържа само *eq*, *започва с* *или* *и* и ограничава всякаква *)* поддръжка, $expand (разширяването на релациите на един обект връща всички релации, но разширяването на колекция от релации на обекти е ограничено)

За повече информация вижте Персонализиране [на отговорите с параметри на заявката](https://docs.microsoft.com/graph/query-parameters).

**API, на който се обаждам, не работи – къде мога да направя повече тестове?**

**Microsoft Graph Explorer** – тествайте API Graph microsoft във вашия клиент или демонстрационен клиент, а също и прегледайте **примерните** заявки в Microsoft Graph Explorer.

**Когато заявка за данни изглежда, че получавам непълен набор от данни обратно**

Ако зададете заявка за колекция (като *например* потребители), Microsoft Graph използва ограничения на страниците от страната на сървъра, така че резултатите винаги да се връщат с размер на страницата по подразбиране. Вашето приложение винаги трябва да очаква да се показва на страница чрез колекции, върнати от услугата.

За повече информация вижте:

- [Най-Graph практики на Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Пейджинг на microsoft Graph данни във вашето приложение](https://docs.microsoft.com/graph/paging)

**Приложението ми е твърде бавно и също се затладява. Какви подобрения мога да направя?**

В зависимост от вашия сценарий има различни опции, с които разполагате, за да направите приложението си по-изпълнително, а в някои случаи по-малко склонни към ограничаване от услугата (когато провеждате твърде много повиквания).

За да научите повече, вижте:

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
