---
title: Разрешаване на вграждането на наследени диалози за отваряне на отчети
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204649"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Разрешаване на вграждането на наследени диалози за отваряне на отчети

**Симптом**

Потребителите не могат да отварят отчети. "Нещо се е объркало. Проверете техническите подробности за повече подробности."

**Причина**

Отчетите не се зареждат в UCI с грешка "Дескриптор на формуляр е null или не е дефиниран." Отчетите в UCI все още изискват наследени диалози, така че системата на клиента трябва да е разрешена *allowlegacydialogsembedding.*

**Решение**

1. Отидете в **раздела Настройки >администриране > Системни настройки > Общи .**

2. Задайте "Разрешаване на вграждането на някои наследени диалогови прозорци в Унифициран интерфейс на браузъра клиент" на **Да**.
