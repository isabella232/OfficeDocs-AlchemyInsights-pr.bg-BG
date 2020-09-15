---
title: ATP за SharePoint, OneDrive и Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715550"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP за SharePoint, OneDrive и Microsoft Teams

Следвайте тези стъпки, за да разрешите разширена защита от заплахи:

1. Отидете на [https://protection.office.com](https://protection.office.com) и влезте с акаунт на глобален администратор или администратор на защитата.

2. В левия навигационния екран под **управление на заплахи**изберете **Policy** \> **безопасни прикачени файлове**за правилата.

3. Изберете **включване на ATP за SharePoint, OneDrive и Microsoft Teams**.

4. [Създайте политика за предупреждения за дейността](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , за да получавате известия, когато откриваме злонамерени файлове.

За пълни инструкции вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Забележка**: по проект ATP не преглежда всеки отделен файл в SharePoint Online, OneDrive за бизнеса или Microsoft Teams. Файловете се сканират асинхронно чрез процес, който използва дейността за споделяне, дейността за гост и сигнали със заплахи за идентифициране на злонамерени файлове. За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
