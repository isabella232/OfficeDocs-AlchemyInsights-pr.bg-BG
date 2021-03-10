---
title: Отстраняване на проблеми с инсталирането на MDATP на Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692861"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Отстраняване на проблеми с инсталирането на MDATP на Mac

Ако ръчно инсталиране е неуспешно, страницата с **Резюме** на съветника за инсталиране показва следната грешка:

"Възникна грешка по време на инсталирането. Инсталиращата програма е срещнала грешка, която е накарала инсталацията да е неуспешна. Свържете се с производителя на софтуера за помощ. "

За разполагания на MDM страницата показва и обща грешка при инсталирането.

Въпреки че не показваме точни грешки на крайните потребители, ние поддържаме регистрационен файл с напредъка на инсталацията в **/Library/logs/Microsoft/mdatp/Install.log**. Всяка сесия за инсталиране се добавя към този регистрационен файл. За да изведете само последната сесия за инсталиране, използвайте `sed` .

За да научите повече, вижте [отстраняване на проблеми с инсталирането за Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
