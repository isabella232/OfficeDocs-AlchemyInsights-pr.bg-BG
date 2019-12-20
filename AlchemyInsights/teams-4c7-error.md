---
title: Грешка в екипите 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795960"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 грешка в екипите на Microsoft

Тази грешка възниква, защото екипите на Microsoft изисква удостоверяване на формуляри. Когато разположите федерация услуги на Active Directory (AD FS), удостоверяване на формуляри не е разрешена за интранет по подразбиране. Ако интегрирано Windows удостоверяване е неуспешно, получавате подкана да влезете с помощта на удостоверяване на формуляри.

За да разрешите този проблем, разрешете удостоверяване на формуляри чрез конзолната добавка AD FS конзолата на Microsoft за управление (MMC) на компютъра с локалното копие на Active Directory. За да направите това, изпълнете следните стъпки: 

1. В навигационния екран прегледайте **правила за удостоверяване**.
2. Под **действия** в екрана с подробни данни изберете **Редактиране на глобално първично удостоверяване**.
3. В раздела **интранет** изберете удостоверяване на **формуляри**.
4. Изберете **OK** (или **Приложете**).