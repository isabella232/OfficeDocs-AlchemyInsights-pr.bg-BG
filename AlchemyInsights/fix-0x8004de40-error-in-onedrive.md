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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525048"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="e9f82-102">Прикрепвам 0x8004de40 грешка в OneDrive</span><span class="sxs-lookup"><span data-stu-id="e9f82-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="e9f82-103">Ако получите грешка 0x8004de40 с OneDrive:</span><span class="sxs-lookup"><span data-stu-id="e9f82-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="e9f82-104">Рестартиране на засегнатите компютър, докато е свързан към домейна си платили директория.</span><span class="sxs-lookup"><span data-stu-id="e9f82-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="e9f82-105">Ако рестартиране не коригира проблема, unjoin и да се присъедини вашето устройство от лазурно АД.</span><span class="sxs-lookup"><span data-stu-id="e9f82-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="e9f82-106">**Забележка**: трябва да бъде във вашата корпоративна мрежа при изпълнение на тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="e9f82-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="e9f82-107">Не извършвайте тези стъпки, когато не можете да се свържете с вашата корпоративна инфраструктура (например, докато пътувате).</span><span class="sxs-lookup"><span data-stu-id="e9f82-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="e9f82-108">Отвори повишени командния ред.</span><span class="sxs-lookup"><span data-stu-id="e9f82-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="e9f82-109">За да отворите повишени командния ред, щракнете върху - **Старт**, с десния бутон върху **команден прозорец**и след това щракнете върху **Изпълни като администратор**.</span><span class="sxs-lookup"><span data-stu-id="e9f82-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="e9f82-110">Въведете *dsregcmd /leave* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e9f82-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="e9f82-111">Когато бъде завършена, въведете *dsregcmd/присъединят* и натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e9f82-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="e9f82-112">Когато приключи, затворете командния ред.</span><span class="sxs-lookup"><span data-stu-id="e9f82-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="e9f82-113">Рестартирайте компютъра и влезте в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e9f82-113">Reboot the computer, and log into OneDrive.</span></span>