---
title: Single-Sign за устройства, присъединени към Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404247"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Еднократна регистрация за устройства, присъединени към Azure Active Directory

Ако имате локална среда на Active Directory (AD) и искате да се присъедините към компютрите си, присъединени към домейна на AD, към Azure AD, можете да постигнете това, като направите хибридно присъединяване към Azure AD. [Как да: Планирането на вашата хибридна реализация на присъединяване към Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за внедряване на хибридно присъединяване на Azure AD във вашата среда.

[Конфигуриране на устройства, присъединени към Azure AD, за локални Single-Sign При използване на Windows Hello за бизнеса](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Проблеми с маркера за основно обновяване (PRT)** Маркерът за основно обновяване (PRT) е ключов артефакт на удостоверяването на Azure AD на устройства с Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android. Това е JSON Web Token (JWT), специално издаден на брокери на маркери на Microsoft от първа страна, за да разрешите еднократната регистрация (SSO) в приложенията, използвани на тези устройства. [В Какво представлява маркерът за](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)основно обновяване? ще ви предоставим подробности как се издава, използва и защитава PRT на устройства с Windows 10.

**WamDefaultSet: YES и AzureADPrt: YES** Тези полета показват дали потребителят е удостоверен успешно с Azure AD при влизане в устройството. Ако стойностите са **НЕ,** може да е дължимо:

- Лош ключ за съхранение в TPM, свързан с устройството при регистрация (проверете KeySignTest, докато се изпълнява повишени).
- Алтернативен ИД на влизане
- HTTP прокси сървърът не е намерен

Отстраняване на неизправности с устройства с помощта на командата dsregcmd – [състояние на SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
