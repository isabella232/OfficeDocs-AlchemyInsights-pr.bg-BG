---
title: Разрешаване Сейф прикачени файлове за SharePoint онлайн, OneDrive и Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332368"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване Сейф прикачени файлове за SharePoint онлайн, OneDrive и Microsoft Teams

1. Като използвате своите идентификационни данни за глобален администратор или администратор на защита, отворете портала на Microsoft 365 Defender и след това отидете на Правила & правила за заплахи <https://security.microsoft.com>  \>  \> **Сейф Прикачени** файлове в **раздела** Правила

   За да отидете директно на **страницата Сейф Прикачени файлове,** използвайте <https://security.microsoft.com/safeattachmentv2> .

2. На страницата **Сейф Прикачени файлове** щракнете върху Глобални **настройки**.
3. В менюто, което се появява, изберете Включване на **Microsoft Defender за Office 365 за SharePoint, OneDrive и Microsoft Teams** и след това изберете **Запиши**.

    **Съвет:** Направете следните стъпки, за да подобрите защитата на Сейф прикачени файлове за SharePoint, OneDrive и Microsoft Teams:
    - За да предотвратите изтеглянето на злонамерени файлове от потребителите, използвайте стойността за параметъра `$true` *DisallowInfectedFileDownload* на кратката команда **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** в SharePoint Online PowerShell. За повече информация вижте Използване [на SharePoint PowerShell, за да предотвратите изтеглянето на злонамерени файлове от потребителите.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Създаване на правила за известяване за открити файлове](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

За повече информация [вж. Сейф Прикачени файлове за Office 365 за SharePoint, OneDrive и Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
