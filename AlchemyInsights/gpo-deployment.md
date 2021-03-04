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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427014"
---
# <a name="gpo-deployment"></a>Разполагане на GPO

Настройките за обектите на потребителя и компютъра в Azure Active Directory Domain Services (Azure AD DS) често се управляват чрез обекти на групови правила (GPOs). Azure AD DS включва вградени GPOs за контейнерите на AADDC и AADDC компютри. Можете да персонализирате тези вградени GPOs, за да конфигурирате груповите правила, ако е необходимо за вашата среда. Членовете на групата на Azure AD DC администраторите имат привилегии за администриране на груповите правила във владение на Azure AD DS и могат също да създават потребителски GPOs и организационни единици. За повече информация относно правилата на групата и как работи, вижте [общ преглед на груповите правила](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

В хибридна среда груповите правила, конфигурирани в локална среда на AD DS, не се синхронизират с Azure AD DS. За да дефинирате настройки за конфигурация за потребители или компютри в Azure AD DS, редактирайте един от GPOs по подразбиране или създайте GPO по избор.

Тази статия [управление на груповите правила](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) ви показва как да инсталирате инструменти за управление на групови правила, как Ton редактирате вградения GPOs и как да създадете потребителски GPOs.
