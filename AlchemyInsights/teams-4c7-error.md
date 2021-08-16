---
title: Teams грешка 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049297"
---
# <a name="4c7-error-in-microsoft-teams"></a>Грешка 4c7 в Microsoft Teams

Тази грешка възниква, защото Microsoft Teams изисква удостоверяване на формуляри. Когато разположите услугите за федериране на Active Directory (AD FS), удостоверяването на формуляри не е разрешено за интранет по подразбиране. Ако Windows интегрираното удостоверяване е неуспешно, ще получите подкана да влезете с помощта на удостоверяване на формуляри.

За да разрешите този проблем, разрешете удостоверяването на формуляри с помощта на конзолната добавка AD FS Microsoft Management Console (MMC) на компютъра, на който е локалното копие на Active Directory. За да направите това, изпълнете следните стъпки: 

1. В навигационния екран отидете на Правила **за удостоверяване**.
2. Под **Действия** в екрана с подробни данни изберете **Редактиране на глобално основно удостоверяване**.
3. В раздела **Интранет** изберете Удостоверяване **на формуляри**.
4. Изберете **OK** (или **Приложи**).