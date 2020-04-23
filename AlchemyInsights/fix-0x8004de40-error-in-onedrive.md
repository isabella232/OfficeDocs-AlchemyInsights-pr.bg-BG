---
title: Fix грешка 0x8004de40 в OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716017"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="eeb3a-102">Fix грешка 0x8004de40 в OneDrive</span><span class="sxs-lookup"><span data-stu-id="eeb3a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="eeb3a-103">Ако получите грешка 0x8004de40 с OneDrive:</span><span class="sxs-lookup"><span data-stu-id="eeb3a-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="eeb3a-104">Рестартирайте засегнатия компютър, докато е свързан с домейна на директорията.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="eeb3a-105">Ако рестартирането не реши проблема, отменете и се присъедини към устройството си от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="eeb3a-106">**Забележка**: Трябва да сте в корпоративната си мрежа, докато изпълнявате тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="eeb3a-107">Не изпълнявайте тези стъпки, когато не можете да се свържете с вашата корпоративна инфраструктура (например, докато пътувате).</span><span class="sxs-lookup"><span data-stu-id="eeb3a-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="eeb3a-108">Отворете команден ред с повишени потребителски права.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="eeb3a-109">За да отворите команден прозорец с администраторски права, щракнете върху - **Старт**, щракнете с десния бутон на мишката върху **командния ред**, след което щракнете върху **Изпълнявай като администратор**.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="eeb3a-110">Въведете *dsregcmd /напуснете* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="eeb3a-111">Когато завършите, въведете *dsregcmd /присъединете се* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="eeb3a-112">Когато завършите, затворете командния ред.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="eeb3a-113">Рестартирайте компютъра и влезте в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eeb3a-113">Reboot the computer, and log into OneDrive.</span></span>