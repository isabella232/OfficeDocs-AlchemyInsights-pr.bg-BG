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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404214"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Проблеми с клиента за регистрация на приложения или проблеми със сертификата

Изтичане на тайната на клиента на приложението?

Независимо как е създадено регистрираното приложение, независимо дали чрез стандартния процес на регистрация в портала за регистрация на приложения, или ако директорът на услугата е създаден във вашия клиент с помощта на съгласие за приложение, ще трябва да се създаде нова тайна на клиента преди изтичането на текущия и актуализиран в кода на свързаното приложение. Максималният период на валидност е 2 години. Като напомняне тайната стойност трябва да бъде записана, тъй като тя повече няма да се вижда, след като напусне страницата "Регистрации на приложения" в портала. За повече информация вижте [Бързо започване: Регистриране на приложение в платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) и [Най-добри практики за платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

За да научите повече, вижте [Създаване на приложение azure AD & на услугата в портала – платформа за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).