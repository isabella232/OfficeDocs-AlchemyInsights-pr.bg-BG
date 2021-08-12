---
title: 0x8004de40 грешка при стартиране на OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946568"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 грешка при стартиране на OneDrive

Ако получите съобщение за **грешка 0x8004de40** когато влезете в OneDrive, рестартирате компютъра, докато сте свързани към вашия домейн на работа или училище. Ако получите тази грешка след рестартирането, опитайте това, докато сте свързани към вашия домейн на работа или училище:

1. Щракнете върху Старт и въведете **cmd** или **команден прозорец**  в полето за търсене, щракнете с десния бутон върху приложението за команден прозорец и изберете  **Изпълнявай като администратор**. Ако получите подкана за парола на администратор или за потвърждение, въведете паролата или щракнете върху **Позволи**.  

2. В прозореца на командния прозорец въведете **dsregcmd /leave**  и изчакайте командата да завърши. След това **въведете dsregcmd /join** и изчакайте командата да завърши.
3. Рестартиране на компютъра.
