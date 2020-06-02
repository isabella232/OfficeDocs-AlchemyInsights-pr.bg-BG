---
title: Идентифициране на IP адрес и клиент в регистрационните файлове за проверка
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508905"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="76d48-102">Идентифициране на IP адрес и клиент в регистрационните файлове за проверка</span><span class="sxs-lookup"><span data-stu-id="76d48-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="76d48-103">IP адрес, който отговаря на дейност от потребител или администратор на Microsoft 365 се показва в регистрите за проверка.</span><span class="sxs-lookup"><span data-stu-id="76d48-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="76d48-104">Информацията за клиента също е регистрирана.</span><span class="sxs-lookup"><span data-stu-id="76d48-104">The client information is also logged.</span></span> <span data-ttu-id="76d48-105">Ето стъпките за идентифициране на тази информация</span><span class="sxs-lookup"><span data-stu-id="76d48-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="76d48-106">Влезте в центъра за съответствие на [& на Microsoft 365 за защита](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="76d48-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="76d48-107">Отидете на страницата **търсене**  >  **на регистрационния файл за проверка.**</span><span class="sxs-lookup"><span data-stu-id="76d48-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="76d48-108">Ако се интересувате от конкретна дейност, изберете я от списъка **с дейности.**</span><span class="sxs-lookup"><span data-stu-id="76d48-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="76d48-109">Ако не, всички дейности ще бъдат върнати за избрания потребител (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="76d48-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="76d48-110">**Забележка**: Някои дейности може да не са налични в менюто **"Дейности";** Обаче тези елементи на проверка ще бъдат върнати, ако е избрано **Покажи резултатите за всички дейности** (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="76d48-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="76d48-111">Укажете потребителското име в полето **Потребители** , изберете подходящия период от време за дейността, след което щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="76d48-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="76d48-112">В резултатите можете да видите IP адреса за тази дейност в екрана с резултати.</span><span class="sxs-lookup"><span data-stu-id="76d48-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="76d48-113">Изберете записа за проверка, за да видите подробна информация в допълнителните **подробности** (например Клиент, Потребител, който е извършил действие и др.).</span><span class="sxs-lookup"><span data-stu-id="76d48-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="76d48-114">За повече информация вижте [Намиране на IP адреса на компютъра, използван за достъп до компрометиран акаунт](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="76d48-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
