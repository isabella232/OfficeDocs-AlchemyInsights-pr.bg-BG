---
title: Прикрепвам 0x8004de40 грешка в OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133966"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="24f57-102">Прикрепвам 0x8004de40 грешка в OneDrive</span><span class="sxs-lookup"><span data-stu-id="24f57-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="24f57-103">Ако получите грешка 0x8004de40 с OneDrive:</span><span class="sxs-lookup"><span data-stu-id="24f57-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="24f57-104">Рестартиране на засегнатите компютър, докато е свързан към домейна си платили директория.</span><span class="sxs-lookup"><span data-stu-id="24f57-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="24f57-105">Ако рестартиране не коригира проблема, unjoin и да се присъедини вашето устройство от лазурно АД.</span><span class="sxs-lookup"><span data-stu-id="24f57-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="24f57-106">**Забележка**: трябва да бъде във вашата корпоративна мрежа при изпълнение на тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="24f57-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="24f57-107">Не извършвайте тези стъпки, когато не можете да се свържете с вашата корпоративна инфраструктура (например, докато пътувате).</span><span class="sxs-lookup"><span data-stu-id="24f57-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="24f57-108">Отвори повишени командния ред.</span><span class="sxs-lookup"><span data-stu-id="24f57-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="24f57-109">За да отворите повишени командния ред, щракнете върху - **Старт**, с десния бутон върху **команден прозорец**и след това щракнете върху **Изпълни като администратор**.</span><span class="sxs-lookup"><span data-stu-id="24f57-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="24f57-110">Въведете *dsregcmd /leave* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="24f57-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="24f57-111">Когато бъде завършена, въведете *dsregcmd/присъединят* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="24f57-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="24f57-112">Когато приключи, затворете командния ред.</span><span class="sxs-lookup"><span data-stu-id="24f57-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="24f57-113">Рестартирайте компютъра и влезте в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="24f57-113">Reboot the computer, and log into OneDrive.</span></span>