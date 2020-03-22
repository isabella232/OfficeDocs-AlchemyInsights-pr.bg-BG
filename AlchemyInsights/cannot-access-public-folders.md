---
title: Публични папки не могат да бъдат достъпни
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891738"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може да се свърже с публични папки

Ако достъпът до публична папка не работи за някои потребители, опитайте следното:

Свързване с EXO PowerShell и конфигуриране на параметъра DefaultPublicFolderMailbox на потребителския акаунт на проблема да съответства на параметъра на работещ потребителски акаунт.

Пример:

Потребител на работа с пощенски кутии | фута по подразбиранеПубличнапапка,ефективнапубличнапапкаПощенска кутия

Задаване на пощенска кутия за \<проблемПотребител -DefaultPublicFolderMailbox стойност от предишна команда>

Изчакайте поне един час, за да влязат в сила промяната.

Ако проблемът остава, моля, следвайте [тази процедура](https://aka.ms/pfcte) за отстраняване на проблеми с публична папка достъп с помощта на Outlook.