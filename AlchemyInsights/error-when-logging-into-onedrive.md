---
title: 0x8004de40 грешка при стартиране на OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813641"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="a7571-102">0x8004de40 грешка при стартиране на OneDrive</span><span class="sxs-lookup"><span data-stu-id="a7571-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="a7571-103">Ако получите съобщение за **грешка 0x8004de40** влизане в OneDrive, рестартирайте компютъра, докато сте свързани към вашия домейн на работа или училище.</span><span class="sxs-lookup"><span data-stu-id="a7571-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="a7571-104">Ако получите тази грешка след рестартирането, опитайте това, докато сте свързани към вашия домейн на работа или училище:</span><span class="sxs-lookup"><span data-stu-id="a7571-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="a7571-105">Щракнете върху Старт и въведете **cmd** или **команден прозорец**  в полето за търсене, щракнете с десния бутон върху приложението за команден прозорец и изберете  **Изпълнявай като администратор**.</span><span class="sxs-lookup"><span data-stu-id="a7571-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="a7571-106">Ако получите подкана за парола на администратор или за потвърждение, въведете паролата или щракнете върху **Позволи**.</span><span class="sxs-lookup"><span data-stu-id="a7571-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="a7571-107">В прозореца на командния прозорец въведете **dsregcmd /leave**  и изчакайте командата да завърши.</span><span class="sxs-lookup"><span data-stu-id="a7571-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="a7571-108">След това **въведете dsregcmd /join** и изчакайте командата да завърши.</span><span class="sxs-lookup"><span data-stu-id="a7571-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="a7571-109">Рестартиране на компютъра.</span><span class="sxs-lookup"><span data-stu-id="a7571-109">Reboot your computer.</span></span>
