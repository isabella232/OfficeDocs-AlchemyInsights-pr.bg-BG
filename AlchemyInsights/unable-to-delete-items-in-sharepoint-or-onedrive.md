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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571222"
---
# <a name="unable-to-delete-items"></a>Не може да се изтрият елементи

Правила за задържане може да доведе до това, трябва да забраните или изключите съответното задържане, което причинява този проблем. След премахването на правило или задържане, може да отнеме до 24 часа, за да влязат в сила промяната. Уверете се, че няма настройка на правила за [задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.

Сайтът може да е надвишил лимита за съхранение, да увеличи [квотата](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) на сайта и да изтрие елемента.

Уверете се, че елементът не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) на друг потребител.

И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), която съдържа библиотека от PowerShell команди, които ви позволяват да извършвате сложни действия за управление като сила изтриване на упорити елементи.
- [Премахване на PNP файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахни папката PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от списък с PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на списък с PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахване на PNP поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)