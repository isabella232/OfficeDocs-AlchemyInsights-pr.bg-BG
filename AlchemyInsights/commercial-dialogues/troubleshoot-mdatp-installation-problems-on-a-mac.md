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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090973"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Отстраняване на проблеми с инсталирането на MDATP на Mac

Ако ръчното инсталиране е неуспешно, **страницата** Резюме на съветника за инсталиране показва следната грешка:

"Възникна грешка по време на инсталирането. Инсталиращата програма се натъкна на грешка, която е причинила неуспешно инсталирането. Обърнете се към производителя на софтуера за помощ".

За разполагания на MDM страницата показва и обща грешка при инсталиране.

Въпреки че не показваме точни грешки на крайните потребители, поддържаме регистрационен файл с напредъка на инсталирането, в **/Library/Logs/Microsoft/mdatp/install.log**. Всяка сесия за инсталиране добавя към този регистрационен файл. За да изведете само последната сесия на инсталиране, използвайте `sed` .

За да научите повече, вижте Отстраняване [на проблеми с инсталирането за Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
