---
title: Влизане в Windows 10 без използване на парола
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107494"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Влизане в Windows 10 без използване на парола

За да избегнете въвеждане на парола при стартиране Windows, ви препоръчваме да използвате една от опциите за Windows Hello защитено влизане, като например ПИН код, разпознаване на лица или пръстов отпечатък, ако има такива. Ако наистина искате да забраните защитеното влизане, вижте инструкциите "Автоматично влизане в Windows 10" по-долу.

**Защитени Windows Hello алтернативи на паролата за акаунта**

Отидете на **Настройки > акаунти > за влизане** (или щракнете [тук](ms-settings:signinoptions?activationSource=GetHelp)). Наличните опции за влизане ще бъдат изброени. Например:

![Опции за влизане.](media/sign-in-options.png)

Щракнете върху или докоснете една от опциите, за да я конфигурирате. Следващия път, когато стартирате или отключите Windows, ще можете да използвате новата опция вместо парола. 

**Автоматично влизане в Windows 10**

**Забележка:** Автоматичното влизане е удобно, но въвежда риск за защитата, особено ако компютърът ви е достъпен от няколко души. 

1. Щракнете върху или докоснете **бутона Старт** в лентата на задачите.

2. Въведете **netplwiz и** натиснете клавиша Enter, за да отворите прозореца Потребителски акаунти.

3. В **Потребителски акаунти** щракнете върху акаунта, в който искате автоматично да влезете, когато Windows стартира.

4. Премахнете отметката от квадратчето "Потребителите трябва да въвеждат потребителско име и парола, за да използват този компютър".

    ![Потребителите трябва да въвеждат опция за потребителско име и парола.](media/users-must-enter-username.png)

5. Щракнете върху **OK**. Ще бъдете помолени да въведете и потвърдите паролата за акаунта, който сте избрали. Щракнете върху **OK,** за да завършите. Следващия път Windows 10 стартира, той автоматично ще влиза в акаунта, който сте избрали.
