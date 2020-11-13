---
title: Не можете да изтривате елементи в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019572"
---
# <a name="unable-to-delete-items"></a>Не могат да се изтрият елементи

- Правилата за съхранение могат да предизвикат това, трябва да забраните или да изключите съответното задържане, което е причина за този проблем. След премахването на правилата за съхранение или задържане, може да са необходими до 24 часа, за да влезе в сила промяната. Уверете се, че няма настройка на [правилата за съхранение](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) в елемента.

- Сайтът може да е надхвърлил ограничението за място за съхранение, да увеличи [квотата за сайта](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) и да изтрие елемента.

- Уверете се, че елементът не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) при друг потребител.

- Накрая администраторите могат да използват [модели и практики на SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), който съдържа библиотека с команди на PowerShell, които ви позволяват да извършвате сложни действия за управление, като например принудително изтриване на упорити елементи.
- [Премахване на PNP файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на PNP папка](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от списък с PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на PNP списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахване на PNP поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)