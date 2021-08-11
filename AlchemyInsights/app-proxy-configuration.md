---
title: Конфигуриране на прокси сървър на приложение
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951554"
---
# <a name="app-proxy-configuration"></a>Конфигуриране на прокси сървър на приложение

1. За да разберете как да конфигурирате приложение за прокси сървър на приложение в Azure AD, за да изложите локалните си приложения в облака, вижте Как да [конфигурирате приложение за прокси сървър на приложение.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Еднократната регистрация (SSO) позволява на потребителите ви достъп до приложение, без да се удостоверяват няколко пъти. Позволява еднократното удостоверяване да се случва в облака, срещу Azure Active Directory и позволява на услугата или Конектора да се представя за потребителя, за да изпълни всички допълнителни предизвикателства пред удостоверяването от приложението. За да научите повече, вижте [Как да конфигурирате еднократната влизане в приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Използвайте [тази статия, за](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) да отстранявате често срещани проблеми, с които хората се сблъскват, когато създават ново приложение за прокси сървър на приложение.
4. Ако имате проблем с настройването на удостоверяването в обратната част на вашето приложение, може да се наложи да отстраните конфигурациите на делегиране, ограничени от [Kerberos,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) за прокси сървър на приложение или да следвате указания за конфигуриране на приложение с [PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) за да решите проблема си.
