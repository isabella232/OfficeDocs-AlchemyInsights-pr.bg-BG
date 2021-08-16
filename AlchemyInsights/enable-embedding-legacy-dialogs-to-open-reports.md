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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003378"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети

**Симптом**

Потребителите не могат да отварят отчети. "Нещо се обърка. Проверете техническите подробности за пояснения."

**Причина**

Отчетите не успяват да се заредят в UCI с грешката "Дескрипторът на формуляра е празен или не е дефиниран". Отчетите в UCI все още изискват наследени диалогови прозорци, така че в системата на клиента трябва да има разрешено *allowlegacydialogsembedding*.

**Решение**

1. Отидете в раздела **Настройки > Администрация > Настройки на системата > Общи**.

2. Задайте "Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети" на **Да**.
