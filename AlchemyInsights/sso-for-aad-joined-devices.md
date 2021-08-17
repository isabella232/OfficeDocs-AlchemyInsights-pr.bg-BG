---
title: Single-Sign за Azure Active Directory присъединени устройства
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049999"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Еднократната регистрация за Azure Active Directory присъединени устройства

Ако имате локална среда на Active Directory (AD) и искате да се присъедините към компютрите си, присъединени към домейна на AD, към Azure AD, можете да постигнете това, като направите хибридно присъединяване към Azure AD. [Как да: Планирането на вашата хибридна Azure Active Directory присъединяване](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за внедряване на хибридно присъединяване на Azure AD във вашата среда.

[Конфигуриране на устройства, присъединени към Azure AD, за локални Single-Sign На Windows Hello за бизнеса](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Проблеми с маркера за основно обновяване (PRT)** Маркерът за основно обновяване (PRT) е ключов артефакт на удостоверяването на Azure AD на Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android. Това е JSON Web Token (JWT), специално издаден на брокери на маркери на Microsoft от първа страна, за да разрешите еднократната регистрация (SSO) в приложенията, използвани на тези устройства. [В Какво представлява маркерът](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)за основно обновяване? , ще предоставим подробности как се издава, използва и защитава PRT на Windows 10 устройства.

**WamDefaultSet: YES и AzureADPrt: YES** Тези полета показват дали потребителят е удостоверен успешно с Azure AD при влизане в устройството. Ако стойностите са **НЕ,** може да е дължимо:

- Лош ключ за съхранение в TPM, свързан с устройството при регистрация (проверете KeySignTest, докато се изпълнява повишени).
- Алтернативен ИД на влизане
- HTTP прокси сървърът не е намерен

Отстраняване на неизправности с устройства с помощта на командата dsregcmd – [състояние на SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
