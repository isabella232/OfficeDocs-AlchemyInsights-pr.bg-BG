---
title: Разрешаване на Office 365 ATP за екипи на SharePoint, OneDrive и Microsoft
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506907"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на разширена защита срещу заплахи за Office 365 за SharePoint Online, OneDrive и екипи на Microsoft

1. Отидете на https://protection.office.com и влезте в профила си.
2. Изберете **Правила за управление на**  >  **Policy**  >  **заплахите Безопасни прикачени файлове**.
3. Изберете **Включване на ATP за SharePoint, OneDrive и Екипи на Microsoft**, след което щракнете върху **Запиши**.
4. (Препоръчително) Като глобален администратор или SharePoint Online администратор, стартирайте кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedFileDownload** настроен на *true.*
5. (Препоръчително) [Настройване на предупреждения](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.

> [!NOTE]
> ATP ще сканира всеки отделен файл в SharePoint Online, OneDrive или екипи на Microsoft. Файловете се сканират асинхронно, чрез процес, който използва събития за споделяне и гост дейност, заедно с интелигентни евристични методи и заплахи за идентифициране на злонамерени файлове. Вижте [ATP за SharePoint, OneDrive и Екипи на Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)