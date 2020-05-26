---
title: Блокиране на изтегляне на връзки за споделяне
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357346"
---
# <a name="block-download-on-sharing-links"></a>Блокиране на изтегляне на връзки за споделяне

**Блокиране на изтегляне** е достъпно за **връзки само** за преглед към документи на Office. Когато изберете тази опция, хората, които получат достъп до файла чрез създадената връзка, няма да виждат опции за изтегляне, отпечатване или копиране на файла.

Администраторите могат да контролират дали настройката "блокиране на изтегляне" се появява само за файлове на Office или не чрез промяна на `BlockDownloadLinksFileType` настройката в кратката команди на [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) или [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
