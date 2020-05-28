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
# <a name="teams-client-crashing"></a><span data-ttu-id="6bad0-102">Клиент на Teams има проблем със срив?</span><span class="sxs-lookup"><span data-stu-id="6bad0-102">Teams client crashing?</span></span>

<span data-ttu-id="6bad0-103">Ако клиентът ви в Teams има проблем със срив, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="6bad0-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="6bad0-104">Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="6bad0-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="6bad0-105">Уверете се, че всички [URL адреси и адресни диапазони](https://docs.microsoft.com/microsoftteams/connectivity-issues) на Microsoft са достъпни.</span><span class="sxs-lookup"><span data-stu-id="6bad0-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="6bad0-106">Влезте с акаунта си на администратор на клиент и проверете [вашето състояние на услугата табло,](https://docs.microsoft.com/office365/enterprise/view-service-health) за да се уверите, че не съществува прекъсване или деградация на услугата.</span><span class="sxs-lookup"><span data-stu-id="6bad0-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="6bad0-107">Деинсталиране и преинсталиране на приложението Teams (връзка)</span><span class="sxs-lookup"><span data-stu-id="6bad0-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="6bad0-108">Намерете папката %appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в тази директория.</span><span class="sxs-lookup"><span data-stu-id="6bad0-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="6bad0-109">[Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталирането на Teams и изберете "Изпълнявай като администратор", ако е възможно).</span><span class="sxs-lookup"><span data-stu-id="6bad0-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="6bad0-110">Ако клиентът ви Teams все още се срива, можете ли да възпроизведете проблема?</span><span class="sxs-lookup"><span data-stu-id="6bad0-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="6bad0-111">Ако е така:</span><span class="sxs-lookup"><span data-stu-id="6bad0-111">If so:</span></span>

1. <span data-ttu-id="6bad0-112">Използвайте "Запис на стъпки", за да заснемете стъпките си.</span><span class="sxs-lookup"><span data-stu-id="6bad0-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="6bad0-113">Затворете всички ненужни или поверителни приложения.</span><span class="sxs-lookup"><span data-stu-id="6bad0-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="6bad0-114">Стартирайте steps Recorder и възпроизвеждане на проблема, докато сте влезли с засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="6bad0-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="6bad0-115">[Съберете отборите регистрационни файлове, които улавят записаните повторения стъпки](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="6bad0-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="6bad0-116">**Забележка**: Уверете се, че сте снети влизане в адреса на засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="6bad0-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="6bad0-117">Събиране на информация за разтоварване и /или повреда кофа (Windows).</span><span class="sxs-lookup"><span data-stu-id="6bad0-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="6bad0-118">Стартиране на Windows Powershell на компютъра, където се случва срив и изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="6bad0-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="6bad0-119">Прикачете файла към вашия случай на поддръжка.</span><span class="sxs-lookup"><span data-stu-id="6bad0-119">Attach the file to your support case.</span></span>
