---
title: Не може да изтрие елементи в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057672"
---
# <a name="unable-to-delete-items"></a>Не може да изтрие елементи

Като проблеми, изтриване на елементи?

- Винаги се уверете, че имате [необходимите разрешения](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) да изтриете елемента или [администраторът на колекцията сайтове](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) опит премахнете елемента.

- Гарантира, че няма настройка на [правила за задържане](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) на елемента.

- Гарантира елемент не е [извлечен](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) при друг потребител.

- И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни управление действия като сила изтриване упорит елементи. 
- [Премахнете PNP файл](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Премахване на PNP папка](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Премахване на елемент от PNP списък](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Премахване на PNP списък](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Премахнете PNP поле (колона)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)