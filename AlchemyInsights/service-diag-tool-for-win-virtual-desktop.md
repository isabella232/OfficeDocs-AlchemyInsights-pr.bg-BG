---
title: Инструмент за диагностика на услуги за виртуален работен плот на Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677174"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="3af2a-102">Инструмент за диагностика на услуги за виртуален работен плот на Windows</span><span class="sxs-lookup"><span data-stu-id="3af2a-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="3af2a-103">Виртуален работен плот на Windows (WVD) предлага диагностичен инструмент, който позволява на администраторите да идентифицират грешки чрез един интерфейс.</span><span class="sxs-lookup"><span data-stu-id="3af2a-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="3af2a-104">Този инструмент регистрира информация, свързана с диагностиката, когато WVD се използва от някого, на когото е присвоена роля на WVD.</span><span class="sxs-lookup"><span data-stu-id="3af2a-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="3af2a-105">Всеки регистър съдържа информация за WVD роля, включена в дейността, съобщенията за грешка, които се показват по време на сесията, и информацията за клиента и потребителя.</span><span class="sxs-lookup"><span data-stu-id="3af2a-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="3af2a-106">Анализът на регистрационни файлове за Azure може да бъде конфигуриран за снемане на регистрационния файл за дейността, създаден от диагностичния инструмент.</span><span class="sxs-lookup"><span data-stu-id="3af2a-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="3af2a-107">Ето как:</span><span class="sxs-lookup"><span data-stu-id="3af2a-107">Here's how:</span></span>

1. <span data-ttu-id="3af2a-108">Създайте работна област за анализ на регистрационни файлове с [портала на Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="3af2a-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="3af2a-109">[Свържете компютрите с Windows към Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="3af2a-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="3af2a-110">Получете ИД на работната област и първичния ключ на работната област.</span><span class="sxs-lookup"><span data-stu-id="3af2a-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="3af2a-111">Съветникът за настройка се нуждае от тази информация, за да конфигурира правилно агента и да се увери, че може да комуникира с монитора на Azure.</span><span class="sxs-lookup"><span data-stu-id="3af2a-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="3af2a-112">[Натиснете диагностични данни в работната област](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="3af2a-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="3af2a-113">Можете да изтласкате диагностични данни от вашия клиент на WVD към анализа на регистрационни файлове за работната област.</span><span class="sxs-lookup"><span data-stu-id="3af2a-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="3af2a-114">[Идентифициране и диагностициране на проблеми](https://go.microsoft.com/fwlink/?linkid=2128338) , които са вътрешни или външни по отношение на WVD.</span><span class="sxs-lookup"><span data-stu-id="3af2a-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="3af2a-115">За да научите повече за конфигурирането на инструмента за диагностика на услуги за WVD, вижте [използване на анализи на регистрационни файлове за функцията за диагностика](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="3af2a-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
