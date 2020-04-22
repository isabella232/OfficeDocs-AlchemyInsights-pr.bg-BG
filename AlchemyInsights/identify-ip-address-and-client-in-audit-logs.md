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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716377"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="7f612-102">Идентифициране на IP адрес и клиент в регистрационните файлове за проверка</span><span class="sxs-lookup"><span data-stu-id="7f612-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="7f612-103">Ip адрес, който отговаря на дейност от потребител или администратор на Microsoft 365 се показва в регистрационните файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="7f612-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="7f612-104">Клиентът също се регистрира.</span><span class="sxs-lookup"><span data-stu-id="7f612-104">The client information is also logged.</span></span> <span data-ttu-id="7f612-105">Ето стъпките за идентифициране на такава информация</span><span class="sxs-lookup"><span data-stu-id="7f612-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="7f612-106">Влезте в центъра за сигурност на [Microsoft 365 & съответствие .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="7f612-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7f612-107">Отидете на страницата **за** > **търсене на регистрационния файл за проверка.**</span><span class="sxs-lookup"><span data-stu-id="7f612-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="7f612-108">Ако се интересувате от конкретна дейност, изберете я от списъка **дейности.**</span><span class="sxs-lookup"><span data-stu-id="7f612-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="7f612-109">Ако не, всички дейности ще бъдат върнати за избрания потребител (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="7f612-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="7f612-110">**Забележка:** Някои дейности може да не са налични в менюто **"Дейности";** обаче тези елементи на проверка ще бъдат върнати, ако е избрана **Показване на резултатите за всички дейности** (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="7f612-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="7f612-111">Задайте потребителското име в полето **Потребители** , изберете подходящия период от време за дейността, след което щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="7f612-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="7f612-112">В резултатите можете да видите IP адреса за тази дейност в екрана с резултатите.</span><span class="sxs-lookup"><span data-stu-id="7f612-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="7f612-113">Изберете записа за проверка, за да видите подробна информация в допълнителното меню **Подробности** (например клиент, потребител, който е извършил действие и т.н.).</span><span class="sxs-lookup"><span data-stu-id="7f612-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="7f612-114">За повече информация вижте [Намиране на IP адреса на компютъра, използван за достъп до компрометиран акаунт](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="7f612-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
