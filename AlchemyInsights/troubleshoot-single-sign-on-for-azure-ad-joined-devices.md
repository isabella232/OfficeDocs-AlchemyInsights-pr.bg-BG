---
title: Отстраняване на неизправности при еднократната регистрация за устройства, присъединени към Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039235"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Отстраняване на неизправности при еднократната регистрация за устройства, присъединени към Azure AD

Ако имате локална среда на Active Directory (AD) и искате да се присъедините към компютрите си, присъединени към домейна на AD, към Azure AD, можете да постигнете това, като направите хибридно присъединяване към Azure AD. [Как да: Планирането на вашата хибридна Azure Active Directory присъединяване](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за внедряване на хибридно присъединяване на Azure AD във вашата среда.

За повече информация вижте Конфигуриране на [устройства, присъединени към Azure AD, за локални Single-Sign При използване на Windows Hello за бизнеса](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Проблеми с маркера за основно обновяване (PRT)**

Маркерът за основно обновяване (PRT) е ключов артефакт на удостоверяването на Azure AD на Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android. Това е JSON Web Token (JWT), специално издаден на брокери на маркери на Microsoft от първа страна, за да разрешите еднократната регистрация (SSO) в приложенията, използвани на тези устройства. За подробности как се издава, използва и защитава PRT на Windows 10 устройства, вижте [Какво представлява маркерът за основно обновяване?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES и AzureADPrt: YES**

Тези полета показват дали потребителят е удостоверен успешно с Azure AD при влизане в устройството. Ако стойностите са **НЕ,** може да се дължи на:

- Лош ключ за съхранение в TPM, свързан с устройството при регистрация (проверете KeySignTest, докато се изпълнява повишени)
- Алтернативен ИД на влизане
- HTTP прокси сървърът не е намерен

За отстраняване на неизправности с устройства, които използват командата dsregcmd, [вижте Състояние на SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
