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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743862"
---
# <a name="fix-transport-rules"></a>Коригиране на транспортни правила

Правилото за пощенския поток по избор е засегнало това съобщение. За да прегледате точното правило, направете следното:

1. В резултатите от представянето под **допълнителна информация** отбележете **GUID** или **името на правилата**.
2. Стартиране на обвивката за управление на Exchange. За повече информация вижте [Отваряне на обвивката за управление на Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Изпълнете тази команда (като използвате GUID от подаването си):  **get-TransportRule-самоличност "GUID" | FL * описание***
4. Прегледайте описанието, за да видите конфигурираните условия, които са засегнали съобщението.

За да научите повече, вижте [get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
