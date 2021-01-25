---
title: Проблеми с връзки и URL адреси
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974187"
---
# <a name="issues-with-links-and-urls"></a>Проблеми с връзки и URL адреси

Пренасочване на URL адреси и отговори (и двата израза могат да се сменят) са URL адресите, използвани от платформата за самоличност на Microsoft, за да се върнат заявени маркери за приложения. За информация за тези URL адреси вижте следните статии:

- [Ситуации на удостоверяване и сценарии за приложения](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – информация за пренасочване на URI адреси в страницата за **регистрация на приложението** за всеки сценарий.
- [Пренасочване на ограничения и ограничения за URL адреси](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Не знам как да регистрирам URL адреса на правилния URI/отговор за моето приложение**

Когато влезете с приложението, което разработвате, ако в диалоговия прозорец за влизане се покаже **AADSTS50011: URL адресът на отговора, зададен в искането, не съответства на URL адресите за отговор, <your app ID> конфигурирани за приложението**, ще трябва да добавите към вашата регистрация на приложението, URI за пренасочване, който използва кодът ви в заявката за идентификация към платформата Microsoft Identity.

За да добавите URL адрес за отговор, отидете в раздела **удостоверяване** на страницата за **регистрация на приложението** в портала на Azure и добавете запис в секцията **пренасочване на URI** . Пренасочване на URI адреси въвеждате (уеб или мобилно/настолно). Стойността, която трябва да въведете, зависи от типа на приложението, което изграждате, както е описано по-долу:

- За приложенията от една страница и уеб приложенията URL адресът на отговора е URL адрес в приложението. Вижте [регистрация на приложения от една страница](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) или [регистрирайте приложение на уеб приложение с помощта на Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- За настолните приложения стойността, която трябва да изберете, зависи от:
    - платформата (MacOS е различна от Windows или Linux)
    - Начинът, по който придобивате маркера (интерактивно, с потока на кода на устройството, с интегрирано удостоверяване на Windows [IWA] или с потребителско име и парола).
    За подробности вижте [настолните приложения – регистрация на приложения – URi за пренасочване](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- За мобилни приложения URI за пренасочване зависи от:
    - платформата (iOS/Android/UWP)
    - информацията, използвана за създаване на вашето приложение, като например ИД на пакета в iOS, и име на пакета и хеширане на подписа на Android приложението Azure Portal за регистрация ще ви помогне. За подробности вижте [Конфигуриране на платформата и пренасочване на URI адреси](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Уеб API и някои от немите начини за придобиване на маркери (IWA и потребителско име/парола) не изискват URI за пренасочване.

**Разположих своето уеб приложение и когато изпробвам разгърнатото приложение, получавам съобщение за несъответствие на URL адрес на отговор**

Можете да добавите пренасочване на URI за всички местоположения, на които разположите своето уеб приложение. За повече информация вижте [регистриране на приложение на уеб приложение чрез портала на Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Добавете URI за пренасочване за местоположение веднага след като разположите приложението в това местоположение.

**Не мога да запиша достатъчно URL адреси за отговор**

Вие сте ISV и имате един или няколко пренасочващи URI адреси за всеки ваш клиент. Искате да мигрирате от ADAL/Azure AD v 1.0 към MSAL/Microsoft Identity Platform и ще достигнете [максималния брой пренасочващи URI адреси](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). За да отстраните това, [Добавете пренасочване на URI към Service принципали](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , които отговарят на всеки от вашите клиенти.
