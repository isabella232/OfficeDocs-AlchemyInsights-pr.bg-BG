---
title: Разполагане на GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067829"
---
# <a name="gpo-deployment"></a>Разполагане на GPO

Настройки обекти на потребители и компютри в Azure Active Directory домейнови услуги (Azure AD DS) често се управляват с помощта на обекти с групови правила (GPOs). Azure AD DS включва вградени GPOs за контейнерите за потребители на AADDC и AADDC компютри. Можете да персонализирате тези вградени GPOs, за да конфигурирате групови правила, както е необходимо за вашата среда. Членовете на групата администратори на Azure AD DC имат привилегии за администриране на групови правила в домейна на Azure AD DS и могат също да създават персонализирани GPOs и организационни единици (OUS). За повече информация относно това какво представлява груповите правила и как работи, вижте Общ [преглед на груповите правила](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

В хибридна среда груповите правила, конфигурирани в локална среда на AD DS, не се синхронизират с Azure AD DS. За да дефинирате настройките за конфигуриране за потребители или компютри в Azure AD DS, редактирайте една от GPO по подразбиране или създайте потребителски GPO.

Тази статия [Управление на групови](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) правила ви показва как да инсталирате инструментите за управление на групови правила, как тонът редактира вградените GPOs и как да създавате персонализирани GPOs.
