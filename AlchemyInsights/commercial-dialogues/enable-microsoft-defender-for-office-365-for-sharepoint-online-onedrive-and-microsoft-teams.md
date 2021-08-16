---
title: Разрешаване на Microsoft Defender за Office 365 за SharePoint онлайн, OneDrive и Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058855"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на Microsoft Defender за Office 365 за SharePoint онлайн, OneDrive и Microsoft Teams

1. Като използвате своите идентификационни данни за глобален администратор или администратор на защита, [влезте в Office 365 за защита и съответствие.](https://protection.office.com/)
2. Изберете **Управление на заплахи** в левия екран и след това изберете Правила **Сейф** прикачени  >  [файлове.](https://protection.office.com/safeattachment)
3. Изберете **Включване на Microsoft Defender за Office 365 за SharePoint, OneDrive** и Microsoft Teams и след това изберете **Запиши**.
    > [!TIP]
    >
    > - Като глобален администратор или администратор на SharePoint Online изпълнете следната кратка команда на PowerShell с **параметъра DisallowInfectedFileDownload,** зададен на *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Настройване на известия за открити файлове](https://go.microsoft.com/fwlink/?linkid=2092110)

За повече информация вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
