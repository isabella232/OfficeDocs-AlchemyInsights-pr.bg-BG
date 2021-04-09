---
title: Коригиране 0x8004de40 грешка в OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649737"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Коригиране 0x8004de40 грешка в OneDrive

Ако изпълнявате Windows 7 и получавате тази грешка, Актуализирайте, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows .

Ако използвате Windows 10 и получите съобщение за грешка 0x8004de40 OneDrive:

- Можете да рестартирате засегнатия компютър, докато сте свързани към домейна си в Acitve Directory.
- Ако рестартирането не коригира проблема, премахнете и се присъедините отново към устройството си от Azure AD. 

**Забележка:** Трябва да сте в корпоративната си мрежа, докато изпълнявате тези стъпки. Не изпълнявайте тези стъпки, когато не сте свързани към вашата корпоративна инфраструктура (например по време на пътуване). 

1. Отворете команден прозорец с повишени права, като **изберете Старт**, щракнете с **десния** бутон върху Команден прозорец и след това **изберете Изпълнявай като администратор**.

1. Въведете *dsregcmd /leave и* натиснете **Enter**.

1. Когато завършите, въведете *dsregcmd /join и* натиснете **Enter**.

1. Когато завършите, затворете командния прозорец.

1. Можете да рестартирате компютъра и да влезете в OneDrive.