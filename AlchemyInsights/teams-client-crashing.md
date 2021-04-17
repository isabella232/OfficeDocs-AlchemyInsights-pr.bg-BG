---
title: Клиент на Teams има проблем със срив?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826260"
---
# <a name="teams-client-crashing"></a>Клиент на Teams има проблем със срив?

Ако клиентът ви в Teams има проблем със срив, опитайте следното:

- Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Уверете се, че всички [URL и адресни диапазони на Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.

- Влезте със своя акаунт за администратор [](https://docs.microsoft.com/office365/enterprise/view-service-health) на клиента и проверете таблото за изтещаване на услугите, за да се уверите, че не съществува излишна работа или влошаване на услугата.

- Деинсталиране и преинсталиране на приложението Teams (връзка)
    - Отидете до папката %appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в този указател.
    - [Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма на Teams и изберете "Изпълнявай като администратор", ако има такива).

Ако вашият клиент на Teams все още се срива, можете ли да възпроизведете проблема? Ако е така:

1. Използвайте "Запис на стъпки", за да заснемете стъпките си.
    - Затворете ВСИЧКИ ненужни или поверителни приложения.
    - Стартирайте "Запис на стъпки" и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.
    - [Събирайте регистрационните файлове на екипите, които заснемат записаните стъпки за повторения.](https://docs.microsoft.com/microsoftteams/log-files) **Забележка:** Уверете се, че заснемате адреса за влизане на засегнатия потребител.
    - Събиране на информацията за дъмп и/или грешка (Windows). Стартирайте Windows Powershell на компютъра, където се случва сривът, и изпълнете следните команди:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Прикачете файла към вашия случай за поддръжка.
