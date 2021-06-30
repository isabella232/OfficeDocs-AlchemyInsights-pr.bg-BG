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
# <a name="teams-client-crashing"></a><span data-ttu-id="0475b-102">Teams клиент се срива</span><span class="sxs-lookup"><span data-stu-id="0475b-102">Teams client crashing</span></span>

<span data-ttu-id="0475b-103">Ако клиентът ви в Teams има проблем със срив, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="0475b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0475b-104">Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0475b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0475b-105">Уверете се, че [всички Microsoft 365 и адресните диапазони](/microsoftteams/connectivity-issues) са достъпни.</span><span class="sxs-lookup"><span data-stu-id="0475b-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0475b-106">Влезте със своя акаунт за администратор [](/office365/enterprise/view-service-health) на клиента и проверете таблото за изтещаване на услугите, за да се уверите, че не съществува излишна работа или влошаване на услугата.</span><span class="sxs-lookup"><span data-stu-id="0475b-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="0475b-107">Деинсталиране и преинсталиране на Teams приложение</span><span class="sxs-lookup"><span data-stu-id="0475b-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="0475b-108">Отидете до папката %appdata%\Microsoft\Teams\ на вашия компютър и изтрийте всички файлове в този указател.</span><span class="sxs-lookup"><span data-stu-id="0475b-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="0475b-109">[Изтеглете и инсталирайте приложението Teams и,](https://www.microsoft.com/microsoft-teams/download-app)ако е възможно, инсталирайте Teams като администратор (щракнете с десния бутон върху инсталиращата програма Teams и изберете **Изпълнявай като администратор, ако** е налично).</span><span class="sxs-lookup"><span data-stu-id="0475b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="0475b-110">Ако вашият Teams все още се срива, опитайте да възпроизведете проблема.</span><span class="sxs-lookup"><span data-stu-id="0475b-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="0475b-111">Ако можете:</span><span class="sxs-lookup"><span data-stu-id="0475b-111">If you can:</span></span>

1. <span data-ttu-id="0475b-112">Използвайте "Запис на стъпки", за да заснемете стъпките си.</span><span class="sxs-lookup"><span data-stu-id="0475b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="0475b-113">Затворете ВСИЧКИ ненужни или поверителни приложения.</span><span class="sxs-lookup"><span data-stu-id="0475b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="0475b-114">Стартирайте "Запис на стъпки" и възпроизведете проблема, докато сте влезли със засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="0475b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="0475b-115">[Събирайте регистрационните файлове на екипите, които заснемат записаните стъпки за повторения.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="0475b-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="0475b-116">**Забележка:** Уверете се, че заснемате адреса за влизане на засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="0475b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="0475b-117">Събиране на информацията за сметището и/или грешката (Windows).</span><span class="sxs-lookup"><span data-stu-id="0475b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="0475b-118">Стартиране Windows Powershell на компютъра, където се случва сривът, и изпълнете следните команди (след всяка команда натиснете Enter):</span><span class="sxs-lookup"><span data-stu-id="0475b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="0475b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="0475b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="0475b-120">След като текстовият файл се генерира и се появи на екрана ви, запишете файла и го прикачете към заявката за услуга.</span><span class="sxs-lookup"><span data-stu-id="0475b-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
