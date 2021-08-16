---
title: Коригиране на транспортни правила
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034743"
---
# <a name="fix-transport-rules"></a>Коригиране на транспортни правила

Това съобщение се отрази на правило за пощенския поток по избор. За да прегледате точното правило, направете следното:

1. В резултатите от подаването, под **Допълнителна информация** обърнете внимание на **GUID** или името **на правилата.**
2. Стартирайте Exchange за управление. За повече информация вижте Отваряне [на обвивката Exchange за управление.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Изпълнете тази команда (като използвате GUID от вашето подаване):  **Get-TransportRule -identity "GUID" | fl * Описание***
4. Прегледайте описанието, за да видите конфигурираните условия, които са повлияли на съобщението.

За да научите повече, вижте [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
