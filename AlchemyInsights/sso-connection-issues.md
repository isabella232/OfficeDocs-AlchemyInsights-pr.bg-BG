---
title: Проблеми със SSO връзката
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084335"
---
# <a name="sso-connection-issues"></a>Проблеми със SSO връзката

1. Следвайте [бързото започване: Конфигуриране на свойства за ръководството на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) за конфигуриране на вашето приложение.
2. В зависимост от опцията за еднократна [регистрация и приложението,](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) която сте избрали, следвайте съответните указания по-долу:
    - За да **конфигурирате локално** приложение за еднократна регистрация, базирана на **SAML,** вж. [SAML еднократна](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)еднократна регистрация за локални приложения с прокси сървър на приложение .
    - За да **конфигурирате приложение в** облака за еднократна еднократна **регистрация,** базирано на парола, вижте  [Конфигуриране на еднократната регистрация с парола](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - За да **конфигурирате локално приложение** за еднократна влизане чрез прокси сървър на приложение, вижте Сводване с парола за еднократна влизане с прокси сървър на [приложение.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
3. **Отстраняване на проблеми с** прокси сървъра на приложение: препоръчваме да започнете с прегледа на потока за отстраняване на неизправности, проблеми с [конектора](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)за прокси сървър на приложението за отстраняване на грешки , за да определите дали конекторите за прокси сървър на приложение са конфигурирани правилно. Ако все още имате проблеми при свързването с приложението, следвайте потока за отстраняване на неизправности в проблеми с приложението ["Прокси сървър на приложението за отстраняване на грешки".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Можете да [идентифицирате проблеми с CORS с](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) помощта на инструментите за отстраняване на грешки в браузъра:
    - Стартирайте браузъра и намерете уеб приложението.
    - Натиснете **F12, за** да изведете конзолата за отстраняване на грешки.
    - Опитайте да възпроизведете транзакцията и прегледайте съобщението на конзолата. Нарушаването на CORS създава грешка в конзолата за произход.
    - Някои проблеми с CORS не могат да бъдат решени, например когато приложението ви пренасочва към login.microsoft.com удостоверяване и маркерът за достъп изтича. Разговорът с CORS след това е неуспешен. Заобиколно решение за този сценарий е да удължите живота на маркера за достъп, за да предотвратите изтичането му по време на сесията на потребителя. За повече информация как да направите това, вижте [Конфигурируеми животи на маркерите в Платформа за самоличност на Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Отстраняване на проблеми с еднократната еднократна регистрация, базирана на **SAML:** препоръчваме да проверите Проблеми при влизане в конфигурирани приложения, базирани на SAML еднократна влизане, за да намерите решенията на проблемите, с които е [най-вероятно](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)да се сблъскате.
5. **Отстраняване на неизправности с** еднократната регистрация, базирана на парола: препоръчваме ви да проверите Отстраняване на неизправности при еднократната еднократна влизане, базирана на парола, в Azure AD, за да намерите решенията за проблемите, с които е [най-вероятно](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)да се сблъскате.
6. За проблеми с връзката, докато използвате VPN, вижте Как да използвате еднократната услуга за влизане [(SSO) през VPN и Wi-Fi връзки.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
