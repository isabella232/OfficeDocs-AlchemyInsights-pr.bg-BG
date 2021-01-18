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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884846"
---
# <a name="configure-ldap"></a>Конфигуриране на LDAP

За да конфигурирате LDAP, направете следното:

1. Проверете състоянието на вашия домейн в [портала на Azure](https://aka.ms/aadds-health).
1. Уверете се, че е наличен валиден абонамент за Azure AD, и услугите за домейни на Azure AD са разрешени.
1. Сертификатът, който е необходим за разрешаване на защитен LDAP, трябва да бъде получен от надежден публичен сертифициращ орган или да бъде самостоятелно подписан сертификат.
1. Проверете дали сертификатът следва необходимите [указания](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Невалиден сертификат**
1. За да подновите сертификат, следвайте стъпките, за да създадете нов сертификат и повторно качване: [конфигурирайте LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. За да отстраните известен проблем със защитени LDAP предупреждения в Azure Active Directory Domain Services, вижте [Разрешаване на LDAP известявания](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
