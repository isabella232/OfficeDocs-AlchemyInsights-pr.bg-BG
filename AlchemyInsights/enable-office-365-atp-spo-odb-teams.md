---
title: Разрешаване на Office 365 ATP за SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709896"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на разширена защита от заплахи за Office 365 за SharePoint Online, OneDrive и Microsoft Teams

1. Отидете на https://protection.office.com и влезте.
2. Изберете **Threat management**за  >  **Policy**  >  **безопасни прикачени файлове**към политиката за управление на заплахи.
3. Изберете **включване на ATP за SharePoint, OneDrive и Microsoft Teams**и след това щракнете върху **Запиши**.
4. Препоръчва Като глобален администратор или администратор на SharePoint Online, изпълнете кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с набора от параметри **DisallowInfectedFileDownload** на *TRUE*.
5. Препоръчва [Настройване на известявания](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за открити файлове.

> [!NOTE]
> ATP ще сканира всеки отделен файл в SharePoint Online, OneDrive или Microsoft Teams. Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и дейността за гост, както и интелигентни евристики и сигнали със заплахи за идентифициране на злонамерени файлове. Вижте [ATP за SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).