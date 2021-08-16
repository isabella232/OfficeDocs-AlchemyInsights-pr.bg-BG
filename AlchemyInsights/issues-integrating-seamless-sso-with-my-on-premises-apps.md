---
title: Проблеми с интегрирането на безпроблемен SSO с моите локални приложения
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028281"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблеми с интегрирането на безпроблемен SSO с моите локални приложения

За да отстраните проблеми с интегрирането на безпроблемна SSO с локални приложения, направете следното:

**Препоръчителни стъпки**

1. За да **конфигурирате локално приложение** за еднократна влизане чрез прокси сървър на приложение, вижте Сводване с парола за еднократна влизане с прокси сървър на [приложение.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
1. **Отстраняване на проблеми с** прокси сървъра на приложение: препоръчваме да започнете с прегледа на потока за отстраняване на неизправности, проблеми с [конектора](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)за прокси сървър на приложението за отстраняване на грешки , за да определите дали конекторите за прокси сървър на приложение са конфигурирани правилно. Ако все още имате проблеми при свързването с приложението, следвайте стъпките за отстраняване на неизправности в проблеми с приложението ["Прокси сървър на приложението за отстраняване на грешки".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Можете да [идентифицирате проблеми с CORS,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) като използвате следните инструменти за отстраняване на грешки в браузъра:
    1. Стартирайте браузъра и намерете уеб приложението.
    1. Натиснете **F12, за** да изведете конзолата за отстраняване на грешки.
    1. Опитайте да възпроизведете транзакцията и прегледайте съобщението на конзолата. Нарушаването на CORS създава грешка в конзолата за произход.
    1. Някои проблеми с CORS не могат да бъдат решени, например когато приложението ви пренасочва към login.microsoftonline.com удостоверяване, а маркерът за достъп изтича. Разговорът с CORS след това е неуспешен. Заобиколно решение за този сценарий е да удължите живота на маркера за достъп, за да предотвратите изтичането му по време на сесията на потребителя. За повече информация как да направите това, вижте [Конфигурируеми животи на маркерите в Платформа за самоличност на Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Препоръчителни документи**

- [Как да конфигурирате еднократната регистрация в приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [ЕДНОКРАТНА еднократна регистрация за локални приложения с прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Разбиране и решаване на Azure Active Directory проблеми с CORS прокси сървъра на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Отстраняване на неизправности с конфигурации на делегиране на Kerberos за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)