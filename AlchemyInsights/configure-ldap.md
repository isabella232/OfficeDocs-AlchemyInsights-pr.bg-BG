---
title: Конфигуриране на LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090401"
---
# <a name="configure-ldap"></a>Конфигуриране на LDAP

За да конфигурирате LDAP, направете следното:

1. Проверете изздраве на вашия домейн в [портала на Azure](https://aka.ms/aadds-health).
1. Уверете се, че е наличен валиден абонамент за Azure AD и azure AD Domain Services е разрешен.
1. Сертификатът, необходим за разрешаване на защитена LDAP, трябва да бъде получен от надежден публичен сертифициращ орган или да бъде самозаписан сертификат.
1. Уверете се, че сертификатът следва [задължителните указания.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Невалиден сертификат**
1. За да подновите сертификат, следвайте стъпките, за да създадете нов сертификат и да презаредите: [Конфигуриране на LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. За да разрешите известен проблем със защитени LDAP предупреждения в домейнови услуги на Azure Active directory, вижте [Разрешаване на LDAP предупреждения](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
