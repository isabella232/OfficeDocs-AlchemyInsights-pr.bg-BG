---
title: Разрешаване на Microsoft Defender за Office 365 за SharePoint Online, OneDrive и Microsoft Teams
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743235"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на Microsoft Defender за Office 365 за SharePoint Online, OneDrive и Microsoft Teams

1. Като използвате своя глобален администратор или идентификационни данни на администратор на защита, влезте в [центъра за защита и съответствие на Office 365](https://protection.office.com/).
2. Изберете **управление на заплахите** в левия екран и след това изберете  >  [безопасни прикачени файлове](https://protection.office.com/safeattachment)за правилата.
3. Изберете **включване на Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams** и след това изберете **Запиши**.
    > [!TIP]
    >
    > - Като глобален администратор или администратор на SharePoint Online, изпълнете следната кратка команда на PowerShell с параметъра **DisallowInfectedFileDownload** , зададен на *TRUE*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Настройване на известявания за открити файлове](https://go.microsoft.com/fwlink/?linkid=2092110)

За повече информация вижте [Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
