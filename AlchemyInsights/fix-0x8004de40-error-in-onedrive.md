---
title: Отстраняване на грешка 0x8004de40 в OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745119"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="940cc-102">Отстраняване на грешка 0x8004de40 в OneDrive</span><span class="sxs-lookup"><span data-stu-id="940cc-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="940cc-103">Ако получите грешка 0x8004de40 с OneDrive:</span><span class="sxs-lookup"><span data-stu-id="940cc-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="940cc-104">Рестартирайте повредения компютър, докато сте свързани към вашия домейн в директорията на Acitve.</span><span class="sxs-lookup"><span data-stu-id="940cc-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="940cc-105">Ако рестартиране не реши проблема, отменете или се Присъединете отново към устройството от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="940cc-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="940cc-106">**Забележка**: трябва да сте във вашата корпоративна мрежа, като изпълните тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="940cc-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="940cc-107">Не правете тези стъпки, когато не можете да се свържете с корпоративната си инфраструктура (например по време на пътуване).</span><span class="sxs-lookup"><span data-stu-id="940cc-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="940cc-108">Отворете команден прозорец с повишени стойности.</span><span class="sxs-lookup"><span data-stu-id="940cc-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="940cc-109">За да отворите командна подкана с повишени стойности, щракнете върху " **Старт**", щракнете с десния бутон върху **команден прозорец**и след това щракнете върху **Изпълнявай като администратор**.</span><span class="sxs-lookup"><span data-stu-id="940cc-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="940cc-110">Въведете *dsregcmd/Leave* и натиснете клавиша **Enter**.</span><span class="sxs-lookup"><span data-stu-id="940cc-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="940cc-111">Когато сте завършили, въведете *dsregcmd/JOIN* и натиснете клавиша **Enter**.</span><span class="sxs-lookup"><span data-stu-id="940cc-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="940cc-112">Когато приключите, затворете командната подкана.</span><span class="sxs-lookup"><span data-stu-id="940cc-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="940cc-113">Рестартирайте компютъра и влезте в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="940cc-113">Reboot the computer, and log into OneDrive.</span></span>