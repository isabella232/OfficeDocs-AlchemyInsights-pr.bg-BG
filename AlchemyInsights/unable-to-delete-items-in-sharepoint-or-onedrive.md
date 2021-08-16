---
title: Не можете да изтриете елементи в SharePoint или OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038506"
---
# <a name="unable-to-delete-items"></a>Не може да се изтрият елементи

- Правилата за съхранение могат да доведат до това, трябва или да забраните, или да изключите съответното задържане, което е причина за този проблем. След като правилата за съхранение или задържане бъдат премахнати, може да отнеме до 24 часа, за да в сила промяната. Уверете се, че няма настройка [на правила за](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) съхранение на елемента.

- Сайтът може да е надхвърлил ограничението за място за съхранение, [да увеличи квотата на](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) сайта и да изтрие елемента.

- Уверете се, че елементът [не е извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) от друг потребител.

- И накрая, администраторите могат да [използват SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) модели и практики (PnP), която съдържа библиотека с команди на PowerShell, които ви позволяват да извършвате сложни действия за управление, като например принудително изтриване на упорити елементи.
- [Премахване на PNP файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на PNP папка](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от списък на PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на PNP списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахване на PNP поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)