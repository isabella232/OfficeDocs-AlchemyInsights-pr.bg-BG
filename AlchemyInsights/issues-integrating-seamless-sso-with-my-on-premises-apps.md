---
title: Проблеми при интегриране на безпроблемно SSO с моите локални приложения
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868642"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблеми при интегриране на безпроблемно SSO с моите локални приложения

За отстраняване на проблеми с интегриране на безпроблемен SSO с локални приложения направете следното:

**Препоръчителни стъпки**

1. За да конфигурирате **локално приложение** за **еднократна идентификация чрез прокси сървър на приложението**, вижте [парола за засвод за еднократна идентификация с прокси сървър на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Отстраняване на проблеми с прокси сървъра за приложения**: препоръчваме ви да започнете с преглеждане на потока за отстраняване на неизправности, [проблеми със свързването на прокси сървъра на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), за да определите дали конекторите за прокси сървъри за приложения са конфигурирани Ако все още имате проблеми със свързването към приложението, следвайте стъпките за отстраняване на неизправности при проблеми с приложението за [прокси сървър на приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Можете да [идентифицирате проблемите с кора](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) с помощта на следните инструменти за отстраняване на грешки в браузъра:
    1. Стартирайте браузъра и отидете до уеб приложението.
    1. Натиснете **F12** , за да изведете конзолата за отстраняване на грешки.
    1. Опитайте да възпроизведете транзакцията и прегледайте съобщението в конзолата. Нарушение на кора произвежда конзола грешка за произход.
    1. Някои проблеми с кора не могат да бъдат разрешени, като например когато приложението пренасочва към login.microsoftonline.com за удостоверяване и маркерът за достъп изтича. След това кора повикването е неуспешно. Заобиколно решение за този сценарий е да удължите срока на валидност на маркера за достъп, за да предотвратите изтичане на срока по време на сесията на потребителя. За повече информация как да направите това, вижте [конфигурируеми животи за маркери в Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Препоръчвани документи**

- [Как да конфигурирате еднократна идентификация в приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML еднократна идентификация за локални приложения чрез прокси сървър на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Разбиране и решаване на проблеми с прокси сървъра на приложението Azure Active Directory кора](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Отстраняване на неизправности при конфигурации на делегиране на Kerberos за прокси сървър за приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)