---
title: Идентифициране на IP адрес и клиент в регистрационните файлове от одита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539018"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="14d17-102">Идентифициране на IP адрес и клиент в регистрационните файлове от одита</span><span class="sxs-lookup"><span data-stu-id="14d17-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="14d17-103">IP адреса, който отговаря на дейност от Office 365 потребител или администратор се показва в регистрационните файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="14d17-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="14d17-104">Информация за клиента се записва.</span><span class="sxs-lookup"><span data-stu-id="14d17-104">The client information is also logged.</span></span> <span data-ttu-id="14d17-105">Тук са стъпките за идентифициране на такава информация</span><span class="sxs-lookup"><span data-stu-id="14d17-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="14d17-106">Влезте в [Office 365 сигурност & съответствие център](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="14d17-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="14d17-107">Отидете на **Търсене на** > **одит регистрационния файл търсене** страница.</span><span class="sxs-lookup"><span data-stu-id="14d17-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="14d17-108">Ако сте заинтересовани от конкретна дейност, изберете го от списъка с **дейности** .</span><span class="sxs-lookup"><span data-stu-id="14d17-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="14d17-109">Ако не, всички дейности ще бъдат върнати на избрания потребител (по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="14d17-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="14d17-110">**Забележка**: някои дейности не може да бъде достъпна в менюто на **дейностите** ; Въпреки това, тези, които одиторски елементи ще бъдат върнати ако **Показват резултати за всички дейности** е избрана (настройката по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="14d17-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="14d17-111">Задайте потребителското име в полето **потребители** , изберете подходящия период от време за дейността и след това щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="14d17-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="14d17-112">В резултатите можете да видите IP адрес за тази дейност в екрана с резултатите.</span><span class="sxs-lookup"><span data-stu-id="14d17-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="14d17-113">Изберете записа на одита да видите подробна информация в **детайли** flyout (например, клиент, потребител, който изпълнява действие, и т.н.).</span><span class="sxs-lookup"><span data-stu-id="14d17-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="14d17-114">За повече информация вижте [намиране на IP адреса на компютъра, използван за достъп до компромис акаунт](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="14d17-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
