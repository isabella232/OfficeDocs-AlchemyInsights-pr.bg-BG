---
title: Отстраняване на неизправности с еднократната идентификация за Azure AD присъединен устройства
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034925"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Отстраняване на неизправности с еднократната идентификация за Azure AD присъединен устройства

Ако имате локална среда за Active Directory (AD) и искате да се присъедините към своя РЕКЛАМен домейн, към който се присъединяват компютрите към Azure AD, можете да постигнете това, като направите хибридно Azure AD съединение. [Как да: планиране Вашият хибриден Azure Active Directory присъединяване към приложението](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за реализиране на хибридна Azure ad съединение във вашата среда.

За повече информация вижте [Конфигуриране на устройства, свързани с AZURE ad, за локални Single-Sign за използване на Windows Hello за бизнеса](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Проблеми в основния маркер за обновяване (PRT)**

Маркерът за първичен обновяване (PRT) е ключов артефакт на Azure AD удостоверяване в Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android. Това е JSON уеб маркер (JWT), специално издадено на брокери на Microsoft First-токен, за да се разреши еднократната идентификация (SSO) между приложенията, използвани за тези устройства. За подробности относно начина, по който даден PRT е издаден, използван и защитен на устройства с Windows 10, вижте [Какво е първичен маркер за обновяване?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: да и AzureADPrt: да**

Тези полета указват дали потребителят е удостоверен успешно в Azure AD при влизане в устройството. Ако стойностите са " **не**", това може да се дължи на:

- Грешен ключ за място за съхранение в TPM, асоцииран с устройството при регистрацията (проверка на KeySignTest при работа с повишени стойности)
- Алтернативен ИД за влизане
- Не е намерен HTTP прокси сървър

За отстраняване на неизправности при устройства с помощта на командата dsregcmd вижте [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
