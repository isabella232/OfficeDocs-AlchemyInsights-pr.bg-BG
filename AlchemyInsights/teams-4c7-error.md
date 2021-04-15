---
title: Грешка в Teams 4c7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786658"
---
# <a name="4c7-error-in-microsoft-teams"></a>Грешка 4c7 в Microsoft Teams

Тази грешка възниква, защото Microsoft Teams изисква удостоверяване на формуляри. Когато разположите услугите за федериране на Active Directory (AD FS), удостоверяването на формуляри не е разрешено за интранет по подразбиране. Ако интегрираното удостоверяване на Windows е неуспешно, ще получите подкана да влезете с помощта на удостоверяване на формуляри.

За да разрешите този проблем, разрешете удостоверяването на формуляри с помощта на конзолната добавка AD FS Microsoft Management Console (MMC) на компютъра, на който е локалното копие на Active Directory. За да направите това, изпълнете следните стъпки: 

1. В навигационния екран отидете на Правила **за удостоверяване**.
2. Под **Действия** в екрана с подробни данни изберете **Редактиране на глобално основно удостоверяване**.
3. В раздела **Интранет** изберете Удостоверяване **на формуляри**.
4. Изберете **OK** (или **Приложи**).