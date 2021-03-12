---
title: Проблеми с връзки и URL адреси
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707871"
---
# <a name="issues-with-links-and-urls"></a>Проблеми с връзки и URL адреси

URL адресите за пренасочване на URI/отговор (и двата израза са взаимозаменяеми) са URL адресите, използвани от платформата за самоличност на Microsoft за връщане на маркерите, поискани от приложението. За повече информация относно тези URL адреси вижте следните статии:

- [Потоци за удостоверяване и сценарии за приложения](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – информация за URI за пренасочване в страницата за **регистриране на приложенията** за всеки сценарий.
- [Ограничения за URI/отговори за пренасочване](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Не знам как да регистрирам правилния URL адрес за URI/отговор за пренасочване за моето приложение**

Ако при влизане с приложението, което разработвате, в диалоговия прозорец за влизане се покаже **AADSTS50011: URL адресът за отговор, зададен в искането, не съответства на URL адресите за отговор, конфигурирани за приложението <your app ID>**, ще трябва да добавите към регистрацията на приложението си този URI за пренасочване, който се използва в кода ви за искането за маркер, изпратено към платформата за самоличност на Microsoft.

За да добавите URL адрес за отговор, посетете раздела **Удостоверяване** в страницата **за регистриране на приложението** в портала на Microsoft Azure и добавете запис в секцията **URI за пренасочване**. Стойността, която трябва да въведете, зависи от типа на приложението, което изграждате, както е описано по-долу:

- За приложения само с една страница и уеб приложения URL адресът за отговор е URL адрес във вашето приложение. Вижте [Регистриране на приложения с една страница](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) или [Регистриране на уеб приложения чрез портала на Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- За настолни приложения стойността, която трябва да изберете, зависи от:
    - платформата (MacOS се различава от Windows и Linux)
    - начина, по който получавате маркера (интерактивно, чрез поток на код за устройството, чрез интегрирано Windows удостоверяване [IWA] или чрез потребителско име/парола).
    За подробности вижте [Настолни приложения – Регистриране на приложения – URI за пренасочване](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- За мобилни приложения URI за пренасочване зависи от:
    - платформата (iOS/Android/UWP)
    - информацията, използвана за създаване на вашето приложение, например ИД на пакета в iOS или името на пакета и хеша на подписа в Android. Регистрацията на приложения в портала на Microsoft Azure ще ви помогне. За подробности вижте [Конфигуриране на платформата и URI за пренасочване](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> За API за уеб и някои негласни начини за придобиване на маркери (IWA и потребителско име/парола) не се изисква URI за пренасочване.

**Разположих уеб приложението и когато го тествам, получавам съобщение за несъответствие в URL адреса за отговор**

Добавете URI за пренасочване за всички местоположения, където разполагате уеб приложението. За повече информация вижте [Регистриране на уеб приложение чрез портала на Microsoft Azure ](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Добавете URI за пренасочване за дадено местоположение веднага щом разположите приложението в това местоположение.

**Не мога да регистрирам достатъчно URL адреси за отговор**

Вие сте НДС и имате един или няколко URI за пренасочване за всеки ваш клиент. Искате да мигрирате от ADAL/Azure AD v1.0 към MSAL/платформата за самоличност на Microsoft и достигате [максималния брой URI за пренасочване](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). За решаване на този проблем [добавете URI за пренасочване към принципалите на услугата,](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) които отговарят на всеки от вашите клиенти.
