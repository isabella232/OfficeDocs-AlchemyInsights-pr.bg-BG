---
title: Разрешаване на Office 365 ATP за SharePoint, OneDrive и екипи на Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703415"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на разширена защита на заплахите за Office 365 за Екипи на SharePoint Online, OneDrive и Microsoft

1. Отиди https://protection.office.com и се впишете.
2. Изберете**Правила за** >  **управление на** > **заплахите Безопасни прикачени файлове**.
3. Изберете **Включване на ATP за SharePoint, OneDrive и Екипи на Microsoft**, след което щракнете върху **Запиши**.
4. (Препоръчва се) Като глобален администратор или администратор на SharePoint Online изпълнете кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedТаФайлИзтегляне** на *true*.
5. (Препоръчва се) [Настройване на предупреждения](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.

> [!NOTE]
> ATP ще сканира всеки един файл в SharePoint Online, OneDrive или Microsoft Екипи. Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и активност на гост, заедно с интелигентни евристични и сигнали за заплахи за идентифициране на злонамерени файлове. Вижте [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).