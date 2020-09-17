---
title: Коментари в Microsoft Planner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 048b63619256c1322837a06115f97127188aec6d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793567"
---
# <a name="comments-in-microsoft-planner"></a>Коментари в Microsoft Planner

Коментарите за задачи в рамките на план се съхраняват в пощенската кутия на Exchange Online за Microsoft 365 Group, свързан с плана.  Когато публикувате коментар по дадена задача, се изпраща имейл известие до папката "Входящи" на групата и ще получите имейл за всеки следващ коментар, направен по тази задача.

Ето някои отговори на често срещани проблеми, свързани с коментари:

- **Потребителите не получават имейли** - коментарите се изпращат до папката "Входящи" на групата, за групата, към която принадлежи планът. За да получи даден потребител имейлите на групата, групата трябва да бъде конфигурирана за изпращане на групови разговори до пощенските кутии на членовете.

- **Коментарите не се записват** - потребителят, който добавя коментара, няма разрешение да изпраща имейл до Microsoft 365 Group. Прочетете [Как работи Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) за повече информация относно този сценарий.

- Показва се грешката **Вече нямате достъп** или **гости не могат да добавят коментари** - потребители гости, които не могат да изпращат имейли до папката "Входящи" на групата, може да виждат това съобщение. За да отстраните проблема, уверете се, че потребителят гост има валиден имейл адрес.

- **Премахнати потребители получават имейли** - ако потребител коментира задача, преди да бъде премахнат от плана, имейл нишката включва потребителя за всеки коментар, направен по задачата.

За подробна информация за коментари с Microsoft Planner вижте [Как работи Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) и [Коментиране на задачи в Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
