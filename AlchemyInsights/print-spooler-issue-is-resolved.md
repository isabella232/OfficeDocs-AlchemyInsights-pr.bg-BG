---
title: Проблемът с спулера за печат е решен
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911327"
---
# <a name="print-spooler-issue-is-resolved"></a>Проблемът с спулера за печат е решен

Ако вашето устройство е актуализирано с Windows 10 **на ОС 19041.329**, може да сте наблюдавали проблем, при който някои принтери не могат да се отпечатат.   Спулерът за печат може да хвърли грешка или неочаквано да се затвори при опит за печат и няма изход от засегнатия принтер. Този проблем е решен в компилация на ОС  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Текущо разследване**

Файлът на услугата за подсистема на локалния орган за защита (LSASS) (**Isass.exe**) може да е неуспешен на някои устройства със съобщението за грешка "Критичен системен процес, C:\WINDOWS\system32\Isass.exe, неуспешен с код на състоянието c0000008. Сега машината трябва да бъде рестартирана".  **Microsoft работи по решение и ще предостави актуализация в предстоящо издание.**

За повече информация вижте известни проблеми [Windows 10 версия 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).