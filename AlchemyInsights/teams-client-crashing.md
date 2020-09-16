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
# <a name="teams-client-crashing"></a><span data-ttu-id="aafeb-102">Клиент на Teams има проблем със срив?</span><span class="sxs-lookup"><span data-stu-id="aafeb-102">Teams client crashing?</span></span>

<span data-ttu-id="aafeb-103">Ако клиентът ви в Teams има проблем със срив, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="aafeb-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="aafeb-104">Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="aafeb-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="aafeb-105">Уверете се, че всички [URL и адресни диапазони за Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.</span><span class="sxs-lookup"><span data-stu-id="aafeb-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="aafeb-106">Влезте със своя акаунт на администратор на клиент и проверете [таблото за изправност на услугите](https://docs.microsoft.com/office365/enterprise/view-service-health) , за да се уверите, че не съществува прекъсване или влошаване на услугата.</span><span class="sxs-lookup"><span data-stu-id="aafeb-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="aafeb-107">Деинсталиране и преинсталиране на приложението Teams (връзка)</span><span class="sxs-lookup"><span data-stu-id="aafeb-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="aafeb-108">Отидете до папката%appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в този указател.</span><span class="sxs-lookup"><span data-stu-id="aafeb-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="aafeb-109">[Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма на Teams и изберете "Изпълнявай като администратор", ако е налично).</span><span class="sxs-lookup"><span data-stu-id="aafeb-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="aafeb-110">Ако вашият клиент за Teams е все още трясък, можете ли да възпроизведете проблема?</span><span class="sxs-lookup"><span data-stu-id="aafeb-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="aafeb-111">Ако е така:</span><span class="sxs-lookup"><span data-stu-id="aafeb-111">If so:</span></span>

1. <span data-ttu-id="aafeb-112">Използвайте инструмента за запис на стъпки, за да заснемете вашите стъпки.</span><span class="sxs-lookup"><span data-stu-id="aafeb-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="aafeb-113">Затворете всички ненужни или поверителни приложения.</span><span class="sxs-lookup"><span data-stu-id="aafeb-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="aafeb-114">Стартирайте инструмента за запис на стъпки и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="aafeb-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="aafeb-115">[Събиране на регистрационни файлове за Teams, които улавят записаните стъпки на възпроизвеждане](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="aafeb-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="aafeb-116">**Забележка**: Уверете се, че сте заснели адреса за влизане на засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="aafeb-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="aafeb-117">Събиране на информация за кофа за дъмп и/или повреда (Windows).</span><span class="sxs-lookup"><span data-stu-id="aafeb-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="aafeb-118">Стартирайте Windows PowerShell на компютъра, където се намира сривът, и изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="aafeb-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="aafeb-119">Прикачете файла към своя казус за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="aafeb-119">Attach the file to your support case.</span></span>
