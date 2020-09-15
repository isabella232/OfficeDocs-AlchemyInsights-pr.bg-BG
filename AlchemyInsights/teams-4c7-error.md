---
title: Грешка в Teams 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700192"
---
# <a name="4c7-error-in-microsoft-teams"></a>грешка на 4c7 в Microsoft Teams

Тази грешка възниква, тъй като Microsoft Teams изисква удостоверяване на формуляри. Когато разположите услуги на Active Directory за федерацията (AD FS), удостоверяването на формуляри не е разрешено за интранет по подразбиране. Ако интегрираното удостоверяване на Windows е неуспешно, получавате подкана да влезете с помощта на удостоверяване на формуляри.

За да отстраните този проблем, разрешете удостоверяване на формуляри с помощта на конзолната добавка за конзола за управление на Microsoft (MMC) на компютъра, на който е локалното копие на Active Directory. За да направите това, изпълнете следните стъпки: 

1. В навигационния екран отидете на **правила за удостоверяване**.
2. Под **действия** в екрана с подробни данни изберете **Редактиране на глобално основно удостоверяване**.
3. В раздела **интранет** изберете удостоверяване на **формуляри**.
4. Изберете **OK** (или **Apply**).