---
title: Коригиране 0x8004de40 грешка в OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649737"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="71d84-102">Коригиране 0x8004de40 грешка в OneDrive</span><span class="sxs-lookup"><span data-stu-id="71d84-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="71d84-103">Ако изпълнявате Windows 7 и получавате тази грешка, Актуализирайте, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows .</span><span class="sxs-lookup"><span data-stu-id="71d84-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="71d84-104">Ако използвате Windows 10 и получите съобщение за грешка 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="71d84-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="71d84-105">Можете да рестартирате засегнатия компютър, докато сте свързани към домейна си в Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="71d84-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="71d84-106">Ако рестартирането не коригира проблема, премахнете и се присъедините отново към устройството си от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="71d84-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="71d84-107">**Забележка:** Трябва да сте в корпоративната си мрежа, докато изпълнявате тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="71d84-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="71d84-108">Не изпълнявайте тези стъпки, когато не сте свързани към вашата корпоративна инфраструктура (например по време на пътуване).</span><span class="sxs-lookup"><span data-stu-id="71d84-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="71d84-109">Отворете команден прозорец с повишени права, като **изберете Старт**, щракнете с **десния** бутон върху Команден прозорец и след това **изберете Изпълнявай като администратор**.</span><span class="sxs-lookup"><span data-stu-id="71d84-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="71d84-110">Въведете *dsregcmd /leave и* натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="71d84-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="71d84-111">Когато завършите, въведете *dsregcmd /join и* натиснете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="71d84-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="71d84-112">Когато завършите, затворете командния прозорец.</span><span class="sxs-lookup"><span data-stu-id="71d84-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="71d84-113">Можете да рестартирате компютъра и да влезете в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="71d84-113">Reboot the computer, and log into OneDrive.</span></span>