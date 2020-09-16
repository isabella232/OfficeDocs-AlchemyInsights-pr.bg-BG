---
title: Изтриване на личен канал за Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730904"
---
# <a name="delete-a-teams-private-channel"></a>Изтриване на личен канал за Teams

Microsoft е наясно с проблем, който изтрива екипен личен канал, ако имате разрешени правила за съхранение на SharePoint за основния сайт на SharePoint. Microsoft работи по корекция. Междувременно можете да използвате следните заобиколни решения, за да изтриете частния канал.

**Изключвате колекцията от екипи/сайтове от правилата за съхранение на SharePoint.**

1. Отидете в портала за администриране на Office 365 и изберете **Покажи всички** в левия навигационен екран.
2. Под **центрове за администриране**отидете на **защита &**  >  правилата за предотвратяване на загуба на**данни**за съответствие  >  **Policy**.
3. Определете правилата, които се отнасят за сайтовете на SharePoint, и променете правилата, така че сайтът на SharePoint за екипа, съдържащ частния канал, да не е включен в правилата за съхранение.
4. Запазете правилата.
    Възможно е да са необходими до 24 часа, за да влязат в сила настройките за правилата.
    След като сайтът бъде изключен, можете да изтриете частния канал.  
    
***Възможно*** е да успеете да изтриете частния канал с помощта на Microsoft Teams на устройството ви с Android. 

За свързана информация в SharePoint вижте [не можете да изтривате елементи в SharePoint Online или OneDrive за бизнеса](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).