---
title: 0x8004de40 грешка при стартиране на OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822991"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 грешка при стартиране на OneDrive

Ако получите съобщение за грешка **0x8004de40** , когато влезете в OneDrive, рестартирайте компютъра, докато се свързвате със своя служебен или учебен домейн. Ако получите тази грешка, след като рестартирате, опитайте това, докато сте свързани със своя служебен или учебен домейн:

1. Щракнете върху Старт и въведете **CMD** или **команден прозорец**  в полето за търсене, щракнете с десния бутон върху приложението Command подкана и изберете  **Изпълнявай като администратор** . Ако получите подкана за въвеждане на парола на администратор или за потвърждение, въведете паролата или щракнете върху **Разреши** .  

2. В прозореца на командната подкана въведете **dsregcmd/Leave**  и изчакайте командата да завърши. След това въведете **dsregcmd/JOIN** и изчакайте командата да завърши.
3. Рестартирайте компютъра си.
