---
title: Отстраняване на проблеми с спулера за печат
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801830"
---
# <a name="print-spooler-issue-is-resolved"></a>Отстраняване на проблеми с спулера за печат

Ако вашето устройство е било актуализирано с Windows 10  **OS компилация 19041,329**, е възможно да сте забелязали проблем, при който някои принтери не могат да се отпечатат. Спулерът за печат може да хвърли съобщение за грешка или да затвори неочаквано при опит за печат, а изходните резултати да не се предоставят от повредения принтер. Този проблем е решен в ос компилация  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Текущо проучване**

Файлът за услуга на подсистемата за системен доставчик на LSASS (**Isass.exe**) може да е неуспешно на някои устройства със съобщение за грешка "критична системен процес, C:\WINDOWS\system32\Isass.exe, неуспешно с код на състояние c0000008. Сега машината трябва да бъде рестартирана.  **Microsoft работи по резолюция и ще предостави актуализация в предстоящо издание.**

За повече информация вижте  [Windows 10 версия 2004 известни проблеми](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).