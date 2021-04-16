---
title: Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814253"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети

**Симптом**

Потребителите не могат да отварят отчети. "Нещо се обърка. Проверете техническите подробности за пояснения."

**Причина**

Отчетите не успяват да се заредят в UCI с грешката "Дескрипторът на формуляра е празен или не е дефиниран". Отчетите в UCI все още изискват наследени диалогови прозорци, така че в системата на клиента трябва да има разрешено *allowlegacydialogsembedding*.

**Решение**

1. Отидете в раздела **Настройки > Администрация > Настройки на системата > Общи**.

2. Задайте "Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети" на **Да**.
