---
title: Няма достъп до публични папки
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959484"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може да се свърже с публични папки

Ако достъп до публична папка не работи за няколко потребители, опитайте следното:

Свързване с ЕКЗО PowerShell и Конфигурирайте пощенската кутия на проблема по подразбиране на проблемния потребителски акаунт да съвпада с един на работен потребителски акаунт.

Пример:

Get-пощенска кутия WorkingUser | Пощенска кутия, ефективна пощенска кутия за Подразбираннопубликуване

Set-пощенска кутия Проблемпотребител-Подразбиранепублична пощенска кутия \<стойност от предишната команда>

Изчакайте поне един час, за да влезе в сила промяната.