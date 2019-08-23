---
title: Не може да изтрие елементи в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558642"
---
# <a name="unable-to-delete-items"></a>Не може да изтрие елементи

Като проблеми, изтриване на елементи на SharePoint?

- Винаги се уверете, че имате [необходимите разрешения](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) да изтриете елемента или [администраторът на колекцията сайтове](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) опит премахнете елемента.

- Гарантира, че няма настройка на [правила за задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.

- Гарантира елемент не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) при друг потребител.

- И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни управление действия като сила изтриване упорит елементи.
- [Премахнете PNP файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на PNP папка](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от PNP списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на PNP списък](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахнете PNP поле (колона)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)