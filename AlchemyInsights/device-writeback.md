---
title: Нефиксирани на устройство
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256675"
---
# <a name="device-writeback"></a>Нефиксирани на устройство

Устройството нефиксирани се използва в следните сценарии:

- Разрешаване на [Windows Hello за бизнеса чрез хибридно разполагане на Trust сертификат](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Разрешаване на условен достъп на базата на устройства към ADFS (защитени приложения на 2012 R2 или по-нова версия)

    > [!NOTE]
    > За устройството нефиксирани се изисква абонамент за Azure AD Premium.

Това осигурява допълнителна защита и увереност, че достъпът до приложенията е разрешен само за надеждни устройства. За повече информация относно условния достъп вижте [управление на риска с условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) и [Настройка на локален условен достъп чрез регистрацията на устройства с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).

За повече информация относно разрешаването на нефиксирани на устройства за устройствата вижте [Разрешаване на Device нефиксирани](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
