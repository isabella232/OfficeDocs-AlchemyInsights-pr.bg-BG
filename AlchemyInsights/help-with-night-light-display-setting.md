---
title: Помощ за настройката за нощно осветление
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404199"
---
# <a name="help-with-the-night-light-display-setting"></a>Помощ за настройката за нощно осветление

За да научите повече за настройките за нощно показване, вижте [Задаване на дисплея за нощно време в Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Ако опциите за нощно осветление са сиви в Настройки, проверете драйвера на дисплея: 

1. Щракнете върху полето за търсене в лентата на задачите и въведете **Диспечер на устройствата** и след това изберете Диспечер на **устройствата** в резултатите от търсенето.
1. Разгънете **Адаптери за дисплей**. 

За съжаление, функцията за нощно осветление не е налична, ако вашето устройство използва драйвер на DisplayLink или драйвер за basic Display.

Функцията за нощно осветление използва най-новата графична технология, така че може да се наложи да актуализирате драйвера на дисплея:  

- Проверете за актуализации, като изберете Стартиране **на**  >  **актуализирането**  >  **на настройките & проверка на**  >  **windows Update** за актуализации на  >  **Windows**.  

ИЛИ

- Посетете уеб сайта за поддръжка на производителя на хардуера, за да изтеглите и инсталирате ръчно най-новите драйвери за показване.

## <a name="reset-night-light-in-the-registry"></a>Нулиране на нощното осветление в системния регистър

Ако актуализирането на драйвера на дисплея не работи, може да се наложи да нулирате нощното осветление в системния регистър.  

**Внимание:** Тази стъпка за отстраняване на неизправности се препоръчва само за напреднали потребители. Ако промените системния регистър неправилно, може да възникнат сериозни проблеми. За допълнителна защита архивирайте системния регистър, преди да го промените, така че да можете да го възстановите, ако възникнат проблеми.

1. В полето за търсене въведете **regedit и** след това изберете **Редактор на системния регистър** в резултатите от търсенето.

1. Отидете на следния ключ от системния регистър: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Експортирайте и след това изтрийте следния подключ:$$windows.data.bluelightreduction.bluelightreductionstate

1. Експортирайте и след това изтрийте следния подключ:$$windows.data.bluelightreduction.settings

1. Рестартирайте Windows и проверете дали са налични опциите за нощно осветление.

