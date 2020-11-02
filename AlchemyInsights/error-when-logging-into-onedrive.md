---
title: 0x8004de40 грешка при стартиране на OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822991"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="f5ccc-102">0x8004de40 грешка при стартиране на OneDrive</span><span class="sxs-lookup"><span data-stu-id="f5ccc-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="f5ccc-103">Ако получите съобщение за грешка **0x8004de40** , когато влезете в OneDrive, рестартирайте компютъра, докато се свързвате със своя служебен или учебен домейн.</span><span class="sxs-lookup"><span data-stu-id="f5ccc-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="f5ccc-104">Ако получите тази грешка, след като рестартирате, опитайте това, докато сте свързани със своя служебен или учебен домейн:</span><span class="sxs-lookup"><span data-stu-id="f5ccc-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="f5ccc-105">Щракнете върху Старт и въведете **CMD** или **команден прозорец**  в полето за търсене, щракнете с десния бутон върху приложението Command подкана и изберете  **Изпълнявай като администратор** .</span><span class="sxs-lookup"><span data-stu-id="f5ccc-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="f5ccc-106">Ако получите подкана за въвеждане на парола на администратор или за потвърждение, въведете паролата или щракнете върху **Разреши** .</span><span class="sxs-lookup"><span data-stu-id="f5ccc-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="f5ccc-107">В прозореца на командната подкана въведете **dsregcmd/Leave**  и изчакайте командата да завърши.</span><span class="sxs-lookup"><span data-stu-id="f5ccc-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="f5ccc-108">След това въведете **dsregcmd/JOIN** и изчакайте командата да завърши.</span><span class="sxs-lookup"><span data-stu-id="f5ccc-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="f5ccc-109">Рестартирайте компютъра си.</span><span class="sxs-lookup"><span data-stu-id="f5ccc-109">Reboot your computer.</span></span>
