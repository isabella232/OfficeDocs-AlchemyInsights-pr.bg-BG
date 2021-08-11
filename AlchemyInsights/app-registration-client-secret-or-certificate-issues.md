---
title: Проблеми с клиента за регистрация на приложения или проблеми със сертификата
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951482"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Проблеми с клиента за регистрация на приложения или проблеми със сертификата

Изтичане на тайната на клиента на приложението?

Независимо как е създадено регистрираното приложение, независимо дали чрез стандартния процес на регистрация в портала за регистрация на приложения, или ако директорът на услугата е създаден във вашия клиент с помощта на съгласие за приложение, ще трябва да се създаде нова тайна на клиента преди изтичането на текущия и актуализиран в кода на свързаното приложение. Максималният период на валидност е 2 години. Като напомняне тайната стойност трябва да бъде записана, тъй като тя повече няма да се вижда, след като напусне страницата "Регистрации на приложения" в портала. За повече информация вижте [Бързо започване: Регистриране на](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) приложение в Платформа за самоличност на Microsoft и [най-добри практики за Платформа за самоличност на Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

За да научите повече, вижте [Създаване на приложение azure AD & на услугата в портала – Платформа за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
