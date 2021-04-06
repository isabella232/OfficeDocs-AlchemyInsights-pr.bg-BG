---
title: Инструмент за диагностика на услуги за виртуален работен плот на Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595457"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="59676-102">Инструмент за диагностика на услуги за виртуален работен плот на Windows</span><span class="sxs-lookup"><span data-stu-id="59676-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="59676-103">Windows Virtual Desktop (WVD) предлага диагностичен инструмент, който позволява на администраторите да идентифицират грешките чрез един интерфейс.</span><span class="sxs-lookup"><span data-stu-id="59676-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="59676-104">Този инструмент регистрира информация, свързана с диагностиката, всеки път, когато WVD се използва от някого, на когото е присвоена WVD роля.</span><span class="sxs-lookup"><span data-stu-id="59676-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="59676-105">Всеки регистрационен файл съдържа информация за WVD ролята, участваща в дейността, съобщенията за грешки, които се показват по време на сесията, и информацията за клиента и потребителя.</span><span class="sxs-lookup"><span data-stu-id="59676-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="59676-106">Azure Log Analytics може да бъде конфигуриран да заснема регистрационния файл на дейността, създаден от диагностичния инструмент, като изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="59676-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="59676-107">Създайте работна област log Analytics с [портала на Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="59676-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="59676-108">[Свързване на компютри с Windows към Монитор на Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="59676-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="59676-109">Получете ИД на работна област и първичния ключ на вашата работна област.</span><span class="sxs-lookup"><span data-stu-id="59676-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="59676-110">Съветникът за настройка се нуждае от тази информация, за да конфигурира правилно агента и да се увери, че може да комуникира с Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="59676-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="59676-111">[Избутайте диагностични данни в работната област.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="59676-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="59676-112">Можете да избутате диагностични данни от вашия WVD клиент към Log Analytics за вашата работна област.</span><span class="sxs-lookup"><span data-stu-id="59676-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="59676-113">[Идентифицирайте и диагностицирайте](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблеми, които са вътрешни или външни във връзка с WVD.</span><span class="sxs-lookup"><span data-stu-id="59676-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="59676-114">За да научите повече за конфигурирането на инструмента за диагностика на услуги за WVD, вижте Използване на анализ на регистрационни файлове за функцията за диагностика.</span><span class="sxs-lookup"><span data-stu-id="59676-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>