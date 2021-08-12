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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964622"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на Microsoft Defender за Office 365 за SharePoint онлайн, OneDrive и Microsoft Teams

1. Отидете и https://protection.office.com влезте.
2. Изберете **Правила за управление на**  >  **заплахи** Сейф прикачени  >  **файлове**.
3. Изберете **Включване на защитника за Office 365 за SharePoint, OneDrive и Microsoft Teams** и след това щракнете върху **Запиши**.
4. (Препоръчва се) Като глобален администратор или администратор на SharePoint Online изпълнете кратката команда [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **параметъра DisallowInfectedFileDownload,** зададен на *true*.
5. (Препоръчва се) [Настройване на известия за](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) открити файлове.

> [!NOTE]
> Microsoft Defender за Office 365 няма да сканира всеки един файл в SharePoint Онлайн, OneDrive или Microsoft Teams. Файловете се сканират асинхронно чрез процес, който използва събития за споделяне и дейности за гости, както и интелигентни уравнения и сигнали за заплахи за идентифициране на злонамерени файлове. Вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).