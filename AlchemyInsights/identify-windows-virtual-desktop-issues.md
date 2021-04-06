---
title: Идентифициране на проблеми с виртуалния работен плот на Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595456"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Идентифициране на проблеми с виртуалния работен плот на Windows

Диагностиката на виртуалния работен плот на Windows използва само една кратка команда на PowerShell, но съдържа много незадължителни параметри, за да ви помогне да стесните и изолирате проблемите. За да започнете: 

1. Изтеглете и импортирайте модула на Windows Virtual Desktop PowerShell. За подробности вижте Кратки команди [за виртуален работен плот на Windows за Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Изпълнете следната кратка команда, за да влезете в акаунта си:
    
    Пример: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**ЗАБЕЛЕЖКА:** Всички заявки, използващи PowerShell, трябва да включват параметрите -UserName или -ActivityID. За възможности за наблюдение вижте Използване [на log Analytics за функцията за диагностика](https://go.microsoft.com/fwlink/?linkid=2126847).

За да филтрирате диагностичните дейности по потребител, изпълнете следната кратка команда:

Пример: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Има списък с филтри, които можете да изпълните, за да диагностицирате проблеми. За да научите повече за диагностицирането на проблеми, вижте [Идентифициране и диагностициране на проблеми с виртуалния работен плот на Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

За да научите повече за често срещаните грешки, вижте [Често срещани грешки senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
