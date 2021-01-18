---
title: Конфигуриране на прокси сървър на приложението
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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884801"
---
# <a name="app-proxy-configuration"></a>Конфигуриране на прокси сървър на приложението

1. За да разберете как да конфигурирате приложение за прокси сървър за приложения в Azure AD, за да изложите вашите локални приложения в облака, вижте [как да конфигурирате приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Еднократната идентификация (SSO) позволява на вашите потребители да имат достъп до приложение без удостоверяване повече от един час. Позволява на единното удостоверяване да се появява в облака, срещу Azure Active Directory и позволява на услугата или съединителя да се представя за потребителя, за да извърши допълнителни предизвикателства за удостоверяване от приложението. За да научите повече, вижте [как да конфигурирате еднократна идентификация в приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Използвайте [тази статия](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) , за да отстраните често срещани проблеми при създаването на ново приложение за прокси сървър на приложения.
4. Ако имате проблем със създаването на обратно удостоверяване към вашето приложение, може да се наложи да [отстраните конфигурациите на делегиране на Kerberos с ограничени права за прокси сървър за приложения](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) или да следвате указания за [Конфигуриране на приложението с PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , за да отстраните проблема си.
