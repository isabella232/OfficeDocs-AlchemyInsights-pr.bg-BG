---
title: Проблеми с SSO връзката
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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935078"
---
# <a name="sso-connection-issues"></a>Проблеми с SSO връзката

1. Следвайте бърз [Старт: Конфигурирай свойствата за](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ръководство за приложения, за да конфигурирате приложението си.
2. В зависимост от избраната от вас [опция за еднократно влизане](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) , следвайте подходящите указания по-долу:
    - За да конфигурирате **локално приложение** за **еднократна идентификация, базирано на SAML**, вижте [SAML за еднократна идентификация за локални приложения чрез прокси сървър на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - За да конфигурирате **приложение в облака** за **еднократна идентификация, базирано на парола**, вижте  [Конфигуриране на еднократна идентификация на парола](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - За да конфигурирате **локално приложение** за **еднократна идентификация чрез прокси сървър на приложението**, вижте [парола за засвод за еднократна идентификация с прокси сървър на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. Отстраняване на проблеми с **прокси сървъра за приложения**: препоръчваме ви да започнете с преглеждане на потока за отстраняване на неизправности, [проблеми със свързването на прокси сървъра на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), за да определите дали конекторите за прокси сървър на приложението са конфигурирани Ако все още имате проблеми със свързването към приложението, следвайте инструкциите за отстраняване на неизправности при проблеми с приложението за [прокси сървъра](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Можете да [идентифицирате проблемите с кора](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) с помощта на инструменти за отстраняване на грешки на браузъра:
    - Стартирайте браузъра и отидете до уеб приложението.
    - Натиснете **F12** , за да изведете конзолата за отстраняване на грешки.
    - Опитайте да възпроизведете транзакцията и прегледайте съобщението в конзолата. Нарушение на кора произвежда конзола грешка за произход.
    - Някои проблеми с кора не могат да бъдат разрешени, като например когато приложението пренасочва към login.microsoft.com за удостоверяване и маркерът за достъп изтича. След това кора повикването е неуспешно. Заобиколно решение за този сценарий е да удължите срока на валидност на маркера за достъп, за да предотвратите изтичане на срока по време на сесията на потребителя. За повече информация как да направите това, вижте [конфигурируеми животи за маркери в Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Отстраняване на неизправности при еднократна идентификация на SAML**: препоръчваме ви [да проверите проблемите, като влезете в базирани на SAML приложения за еднократна идентификация](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), за да намерите решенията за проблемите, за които най-вероятно ще срещнете.
5. **Отстраняване на неизправности при еднократна идентификация на парола**: препоръчваме ви да проверите [отстраняване на неизправности при еднократна идентификация на базата на парола в Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), за да намерите решенията за проблемите, с които се сблъсквате най-често.
6. За проблеми с връзката, когато използвате VPN, вижте [как да използвате еднократна идентификация (SSO) през VPN и връзки с Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
