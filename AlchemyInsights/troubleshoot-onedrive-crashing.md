---
title: Отстраняване на неизправности в OneDrive се срива
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826188"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="9a417-102">Отстраняване на неизправности в OneDrive се срива</span><span class="sxs-lookup"><span data-stu-id="9a417-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="9a417-103">Ако OneDrive неколкократно се срива, изпробвайте следните стъпки за отстраняване на неизправности:</span><span class="sxs-lookup"><span data-stu-id="9a417-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="9a417-104">**Уверете се, че ключовете от системния регистър не са зададени:**</span><span class="sxs-lookup"><span data-stu-id="9a417-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="9a417-105">С помощта на редактора на системния регистър навигирайте до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="9a417-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="9a417-106">Ако DisableFileSyncNGSC е наличен и зададен на 1, отворете ключа и променете стойността на 0.</span><span class="sxs-lookup"><span data-stu-id="9a417-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="9a417-107">Ръчно стартиране на OneDrive, като отивате в "Старт"</span><span class="sxs-lookup"><span data-stu-id="9a417-107">Manually launch OneDrive by going to Start</span></span> ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="9a417-109">въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a417-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="9a417-110">**Нулиране на OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="9a417-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="9a417-111">Бележки:</span><span class="sxs-lookup"><span data-stu-id="9a417-111">Notes:</span></span>

- <span data-ttu-id="9a417-112">Нулирането на OneDrive прекъсва всички съществуващи връзки за синхронизиране (включително вашия личен OneDrive, ако е настроен).</span><span class="sxs-lookup"><span data-stu-id="9a417-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="9a417-113">Няма да загубите файлове или данни, като нулирате OneDrive на компютъра си.</span><span class="sxs-lookup"><span data-stu-id="9a417-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="9a417-114">**За да нулирате OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="9a417-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="9a417-115">Отворете диалоговия прозорец Изпълнение, като натиснете клавиша Windows и R.</span><span class="sxs-lookup"><span data-stu-id="9a417-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="9a417-116">Въведете %localappdata%\Microsoft\OneDrive\onedrive.exe/reset и натиснете OK.</span><span class="sxs-lookup"><span data-stu-id="9a417-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="9a417-117">За кратко може да се покаже команден прозорец.</span><span class="sxs-lookup"><span data-stu-id="9a417-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="9a417-118">Ръчно стартиране на OneDrive, като отивате в "Старт"</span><span class="sxs-lookup"><span data-stu-id="9a417-118">Manually launch OneDrive by going to Start</span></span> ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="9a417-120">въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a417-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="9a417-121">Бележки:</span><span class="sxs-lookup"><span data-stu-id="9a417-121">Notes:</span></span>

- <span data-ttu-id="9a417-122">Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизирането завърши.</span><span class="sxs-lookup"><span data-stu-id="9a417-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="9a417-123">Прочетете [Изберете кои папки на OneDrive да синхронизирате с вашия компютър](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)за повече   информация.</span><span class="sxs-lookup"><span data-stu-id="9a417-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="9a417-124">Ще трябва да завършите това за вашия личен OneDrive и OneDrive за бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9a417-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>