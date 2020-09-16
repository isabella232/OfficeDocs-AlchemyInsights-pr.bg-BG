---
title: Клиент на Teams има проблем със срив?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691096"
---
# <a name="teams-client-crashing"></a>Клиент на Teams има проблем със срив?

Ако клиентът ви в Teams има проблем със срив, опитайте следното:

- Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Уверете се, че всички [URL и адресни диапазони за Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.

- Влезте със своя акаунт на администратор на клиент и проверете [таблото за изправност на услугите](https://docs.microsoft.com/office365/enterprise/view-service-health) , за да се уверите, че не съществува прекъсване или влошаване на услугата.

- Деинсталиране и преинсталиране на приложението Teams (връзка)
    - Отидете до папката%appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в този указател.
    - [Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма на Teams и изберете "Изпълнявай като администратор", ако е налично).

Ако вашият клиент за Teams е все още трясък, можете ли да възпроизведете проблема? Ако е така:

1. Използвайте инструмента за запис на стъпки, за да заснемете вашите стъпки.
    - Затворете всички ненужни или поверителни приложения.
    - Стартирайте инструмента за запис на стъпки и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.
    - [Събиране на регистрационни файлове за Teams, които улавят записаните стъпки на възпроизвеждане](https://docs.microsoft.com/microsoftteams/log-files). **Забележка**: Уверете се, че сте заснели адреса за влизане на засегнатия потребител.
    - Събиране на информация за кофа за дъмп и/или повреда (Windows). Стартирайте Windows PowerShell на компютъра, където се намира сривът, и изпълнете следните команди:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Прикачете файла към своя казус за поддръжка.
