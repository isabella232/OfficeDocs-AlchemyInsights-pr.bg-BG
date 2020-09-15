---
title: Идентифициране на IP адрес и клиент в регистрационни файлове за проверка
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668299"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ef4f1-102">Идентифициране на IP адрес и клиент в регистрационни файлове за проверка</span><span class="sxs-lookup"><span data-stu-id="ef4f1-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ef4f1-103">IP адресът, който отговаря на дейност от потребител или администратор на Microsoft 365, е показан в регистрационните файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="ef4f1-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ef4f1-104">Информацията за клиента също е регистрирана.</span><span class="sxs-lookup"><span data-stu-id="ef4f1-104">The client information is also logged.</span></span> <span data-ttu-id="ef4f1-105">Ето стъпките за идентифициране на тази информация</span><span class="sxs-lookup"><span data-stu-id="ef4f1-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ef4f1-106">Влезте в центъра за [съответствие на & на Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ef4f1-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ef4f1-107">Отидете на страницата **Search**за  >  **търсене в регистрационния файл за проверка** на търсенето.</span><span class="sxs-lookup"><span data-stu-id="ef4f1-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ef4f1-108">Ако се интересувате от конкретна дейност, изберете я от списъка с **дейности** .</span><span class="sxs-lookup"><span data-stu-id="ef4f1-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ef4f1-109">Ако не, всички дейности ще бъдат върнати за избрания потребител (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="ef4f1-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ef4f1-110">**Забележка**: определени дейности може да не са налични в менюто **дейности** ; обаче тези елементи за проверка ще бъдат върнати, ако са избрани **Покажи резултатите за всички дейности** (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="ef4f1-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ef4f1-111">Задайте потребителското име в полето **потребители** , изберете подходящия диапазон от дати за дейността и след това щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="ef4f1-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ef4f1-112">В резултатите можете да видите IP адреса за тази дейност в екрана резултати.</span><span class="sxs-lookup"><span data-stu-id="ef4f1-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ef4f1-113">Изберете одитния запис, за да видите подробна информация в изплаващо за **подробни данни** (например клиент, потребител, който е извършил действие и т. н.).</span><span class="sxs-lookup"><span data-stu-id="ef4f1-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ef4f1-114">За повече информация вижте [намиране на IP адреса на компютъра, който се използва за достъп до компрометиран акаунт](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="ef4f1-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
