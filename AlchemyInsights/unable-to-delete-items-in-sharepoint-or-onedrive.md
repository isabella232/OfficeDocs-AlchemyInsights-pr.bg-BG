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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049506"
---
# <a name="unable-to-delete-items"></a>Не могат да се изтрият елементи

Имате проблеми с изтриването на елементи на SharePoint?

- Винаги се уверете, че имате [съответните разрешения](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) за изтриване на елемента или имате опит да премахнете този елемент от [администратора на колекцията от сайтове](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .

- Уверете се, че няма настройка на [правилата за задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.

- Уверете се, че елементът не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) за друг потребител.

- И накрая, администраторите могат да използват [модели и практики на SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни управленски действия като сила изтриване на упорити елементи.
- [Премахване на ПНП файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на ПНП папка](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахни ПНП елемент от списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на ПНП списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахване на ПНП поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)