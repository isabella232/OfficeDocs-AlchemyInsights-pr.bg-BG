---
title: Fix 0x8004de40 грешка в OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755837"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a8580-102">Fix 0x8004de40 грешка в OneDrive</span><span class="sxs-lookup"><span data-stu-id="a8580-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a8580-103">Ако получите грешка 0x8004de40 с OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a8580-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a8580-104">Рестартирайте засегнатия компютър, докато сте свързани към домейна на директорията.</span><span class="sxs-lookup"><span data-stu-id="a8580-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a8580-105">Ако рестартиране не реши проблема, премахнете присъединяване и се присъедини към вашето устройство от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a8580-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a8580-106">**Забележка**: трябва да сте в корпоративната си мрежа, докато изпълнявате тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="a8580-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a8580-107">Не извършвайте тези стъпки, когато не можете да се свържете с корпоративната си инфраструктура (например по време на пътуване).</span><span class="sxs-lookup"><span data-stu-id="a8580-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="a8580-108">Отворете команден ред с повишени администраторски права.</span><span class="sxs-lookup"><span data-stu-id="a8580-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="a8580-109">За да отворите команден ред с повишени права, щракнете върху **Старт**, щракнете с десния бутон върху **командния ред**и след това щракнете върху **Изпълнявай като администратор**.</span><span class="sxs-lookup"><span data-stu-id="a8580-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="a8580-110">Въведете *dsregcmd/отпуск* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a8580-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="a8580-111">Когато завършите, въведете *dsregcmd/съединение* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a8580-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="a8580-112">Когато завършите, затворете командния ред.</span><span class="sxs-lookup"><span data-stu-id="a8580-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="a8580-113">Рестартирайте компютъра и влезте в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a8580-113">Reboot the computer, and log into OneDrive.</span></span>