---
title: Teams клиент се срива
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187710"
---
# <a name="teams-client-crashing"></a>Teams клиент се срива

Ако клиентът ви в Teams има проблем със срив, опитайте следното:

- Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Уверете се, че [всички Microsoft 365 и адресните диапазони](/microsoftteams/connectivity-issues) са достъпни.

- Влезте със своя акаунт за администратор [](/office365/enterprise/view-service-health) на клиента и проверете таблото за изтещаване на услугите, за да се уверите, че не съществува излишна работа или влошаване на услугата.

- Деинсталиране и преинсталиране на Teams приложение
    - Отидете до папката %appdata%\Microsoft\Teams\ на вашия компютър и изтрийте всички файлове в този указател.
    - [Изтеглете и инсталирайте приложението Teams и,](https://www.microsoft.com/microsoft-teams/download-app)ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма Teams и изберете **Изпълнявай като администратор, ако** е налично).

Ако вашият Teams все още се срива, опитайте да възпроизведете проблема. Ако можете:

1. Използвайте "Запис на стъпки", за да заснемете стъпките си.
    - Затворете ВСИЧКИ ненужни или поверителни приложения.
    - Стартирайте "Запис на стъпки" и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.
    - [Събирайте регистрационните файлове на екипите, които заснемат записаните стъпки за повторения.](/microsoftteams/log-files) **Забележка:** Уверете се, че заснемате адреса за влизане на засегнатия потребител.
    - Събиране на информацията за сметището и/или грешката (Windows). Стартиране Windows Powershell на компютъра, където се случва сривът, и изпълнете следните команди (след всяка команда натиснете Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. След като текстовият файл се генерира и се появи на екрана ви, запишете файла и го прикачете към заявката за услуга. 
