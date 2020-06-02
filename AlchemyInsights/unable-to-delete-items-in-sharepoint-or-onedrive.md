---
title: Не може да се изтрият елементи в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511965"
---
# <a name="unable-to-delete-items"></a>Не може да се изтрият елементи

Правилата за задържане могат да причинят това, трябва да забраните или изключите съответното задържане, което причинява този проблем. След като правило за задържане или задържане е премахната, промяната може да отнеме до 24 часа. Уверете се, че няма настройка на [правилата за задържане](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) на елемента.

Сайтът може да е надвишил ограничението за съхранение, да увеличи [квотата](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) на сайта и да изтрие елемента.

Уверете се, че елементът не е [извлечен от](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) друг потребител.

И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни действия за управление като принудително изтриване на упорити елементи.
- [Премахване на PNP файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на PNP папка](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от списъка с PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на списъка с PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахване на PNP поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)