---
title: Разрешаване Office 365 ATP за SharePoint, OneDrive и Microsoft Teams
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332148"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на Microsoft Defender за Office 365 за SharePoint онлайн, OneDrive и Microsoft Teams

1. Отидете и https://protection.office.com влезте.
2. Изберете **Правила за управление на**  >  **заплахи** Сейф прикачени  >  **файлове**.
3. Изберете **Включване на защитника за Office 365 за SharePoint, OneDrive** и Microsoft Teams и след това щракнете върху **Запиши**.
4. (Препоръчва се) Като глобален администратор или администратор на SharePoint Online изпълнете кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedFileDownload,** зададен на *true*.
5. (Препоръчва се) [Настройване на известия за](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) открити файлове.

**Забележка:** Microsoft Defender за Office 365 няма да сканира всеки един файл в SharePoint Online, OneDrive или Microsoft Teams. Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и дейности за гости, както и интелигентни уравнения и сигнали за заплахи за идентифициране на злонамерени файлове. Вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
