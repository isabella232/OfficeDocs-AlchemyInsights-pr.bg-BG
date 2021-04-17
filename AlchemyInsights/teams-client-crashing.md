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
# <a name="teams-client-crashing"></a><span data-ttu-id="37cd1-102">Клиент на Teams има проблем със срив?</span><span class="sxs-lookup"><span data-stu-id="37cd1-102">Teams client crashing?</span></span>

<span data-ttu-id="37cd1-103">Ако клиентът ви в Teams има проблем със срив, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="37cd1-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="37cd1-104">Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="37cd1-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="37cd1-105">Уверете се, че всички [URL и адресни диапазони на Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.</span><span class="sxs-lookup"><span data-stu-id="37cd1-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="37cd1-106">Влезте със своя акаунт за администратор [](https://docs.microsoft.com/office365/enterprise/view-service-health) на клиента и проверете таблото за изтещаване на услугите, за да се уверите, че не съществува излишна работа или влошаване на услугата.</span><span class="sxs-lookup"><span data-stu-id="37cd1-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="37cd1-107">Деинсталиране и преинсталиране на приложението Teams (връзка)</span><span class="sxs-lookup"><span data-stu-id="37cd1-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="37cd1-108">Отидете до папката %appdata%\Microsoft\teams\ на вашия компютър и изтрийте всички файлове в този указател.</span><span class="sxs-lookup"><span data-stu-id="37cd1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="37cd1-109">[Изтеглете и инсталирайте приложението Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)и ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма на Teams и изберете "Изпълнявай като администратор", ако има такива).</span><span class="sxs-lookup"><span data-stu-id="37cd1-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="37cd1-110">Ако вашият клиент на Teams все още се срива, можете ли да възпроизведете проблема?</span><span class="sxs-lookup"><span data-stu-id="37cd1-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="37cd1-111">Ако е така:</span><span class="sxs-lookup"><span data-stu-id="37cd1-111">If so:</span></span>

1. <span data-ttu-id="37cd1-112">Използвайте "Запис на стъпки", за да заснемете стъпките си.</span><span class="sxs-lookup"><span data-stu-id="37cd1-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="37cd1-113">Затворете ВСИЧКИ ненужни или поверителни приложения.</span><span class="sxs-lookup"><span data-stu-id="37cd1-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="37cd1-114">Стартирайте "Запис на стъпки" и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="37cd1-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="37cd1-115">[Събирайте регистрационните файлове на екипите, които заснемат записаните стъпки за повторения.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="37cd1-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="37cd1-116">**Забележка:** Уверете се, че заснемате адреса за влизане на засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="37cd1-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="37cd1-117">Събиране на информацията за дъмп и/или грешка (Windows).</span><span class="sxs-lookup"><span data-stu-id="37cd1-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="37cd1-118">Стартирайте Windows Powershell на компютъра, където се случва сривът, и изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="37cd1-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="37cd1-119">Прикачете файла към вашия случай за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="37cd1-119">Attach the file to your support case.</span></span>
