---
title: Отстраняване на неизправности при OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664987"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="0bcc7-102">Отстраняване на неизправности при OneDrive</span><span class="sxs-lookup"><span data-stu-id="0bcc7-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="0bcc7-103">Ако OneDrive се срива многократно, изпробвайте тези стъпки за отстраняване на неизправности:</span><span class="sxs-lookup"><span data-stu-id="0bcc7-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="0bcc7-104">**Проверете дали ключовете на системния регистър не са зададени:**</span><span class="sxs-lookup"><span data-stu-id="0bcc7-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="0bcc7-105">Чрез редактора на системния регистър отидете до HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="0bcc7-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="0bcc7-106">Ако DisableFileSyncNGSC е наличен и зададен на 1, отворете ключа и променете стойността на 0.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="0bcc7-107">Ръчно стартиране на OneDrive, като отидете в "Старт"</span><span class="sxs-lookup"><span data-stu-id="0bcc7-107">Manually launch OneDrive by going to Start</span></span> ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="0bcc7-109">, въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="0bcc7-110">**Нулиране на OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="0bcc7-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="0bcc7-111">Бележки</span><span class="sxs-lookup"><span data-stu-id="0bcc7-111">Notes:</span></span>

- <span data-ttu-id="0bcc7-112">Нулирането на OneDrive прекъсва всички ваши съществуващи връзки за синхронизиране (включително вашия личен OneDrive, ако е настроен).</span><span class="sxs-lookup"><span data-stu-id="0bcc7-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="0bcc7-113">Няма да загубите файлове или данни, като нулирате OneDrive на вашия компютър.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="0bcc7-114">**За нулиране на OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="0bcc7-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="0bcc7-115">Отворете диалоговия прозорец за изпълнение, като натиснете клавиша Windows и R.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="0bcc7-116">Въведете% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset и натиснете OK.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="0bcc7-117">За кратко може да се появи команден прозорец.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="0bcc7-118">Ръчно стартиране на OneDrive, като отидете в "Старт"</span><span class="sxs-lookup"><span data-stu-id="0bcc7-118">Manually launch OneDrive by going to Start</span></span> ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="0bcc7-120">, въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="0bcc7-121">Бележки</span><span class="sxs-lookup"><span data-stu-id="0bcc7-121">Notes:</span></span>

- <span data-ttu-id="0bcc7-122">Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизирането завърши.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="0bcc7-123">Прочетете [Изберете кои папки на OneDrive да се синхронизират с вашия компютър](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   за повече информация.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="0bcc7-124">Ще трябва да изпълните това за своя личен OneDrive и OneDrive за бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0bcc7-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>