---
title: Клиент на Teams има проблем със срив?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354041"
---
# <a name="teams-client-crashing"></a>Клиент на Teams има проблем със срив?

Ако клиентът ви в Teams има проблем със срив, опитайте следното:

- Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Уверете се, че всички [URL адреси и адресни диапазони](https://docs.microsoft.com/microsoftteams/connectivity-issues) на Microsoft са достъпни.

- Влезте с акаунта си на администратор на клиент и проверете [вашето състояние на услугата табло,](https://docs.microsoft.com/office365/enterprise/view-service-health) за да се уверите, че не съществува прекъсване или деградация на услугата.

- Деинсталиране и преинсталиране на приложението Teams (връзка)
    - Намерете папката %appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в тази директория.
    - [Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталирането на Teams и изберете "Изпълнявай като администратор", ако е възможно).

Ако клиентът ви Teams все още се срива, можете ли да възпроизведете проблема? Ако е така:

1. Използвайте "Запис на стъпки", за да заснемете стъпките си.
    - Затворете всички ненужни или поверителни приложения.
    - Стартирайте steps Recorder и възпроизвеждане на проблема, докато сте влезли с засегнатия потребителски акаунт.
    - [Съберете отборите регистрационни файлове, които улавят записаните повторения стъпки](https://docs.microsoft.com/microsoftteams/log-files). **Забележка**: Уверете се, че сте снети влизане в адреса на засегнатия потребител.
    - Събиране на информация за разтоварване и /или повреда кофа (Windows). Стартиране на Windows Powershell на компютъра, където се случва срив и изпълнете следните команди:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Прикачете файла към вашия случай на поддръжка.
