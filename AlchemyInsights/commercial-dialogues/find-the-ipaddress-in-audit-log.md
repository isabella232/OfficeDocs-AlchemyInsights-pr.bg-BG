---
title: Намиране на IP адреса в регистрационен файл за проверка
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481056"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="2fd7b-102">Намиране на IP адреса в регистрационен файл за проверка</span><span class="sxs-lookup"><span data-stu-id="2fd7b-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="2fd7b-103">IP адресът, който отговаря на дейност, изпълнена от потребител или администратор, се показва в регистрационните файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="2fd7b-104">Информацията за клиента също е регистрирана.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-104">The client information is also logged.</span></span> <span data-ttu-id="2fd7b-105">Ето как да идентифицирате IP адрес:</span><span class="sxs-lookup"><span data-stu-id="2fd7b-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="2fd7b-106">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="2fd7b-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="2fd7b-107">Изберете **търсене** в  >  **[регистрационния файл за проверка](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="2fd7b-108">Ако видите съобщение, което ви трябва, за да включите проверката, продължете напред и го включете сега.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="2fd7b-109">Ако тази функция не е разрешена, резултатите от търсенето няма да могат да изтеглят данни от предишни дати.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="2fd7b-110">Ако се интересувате от конкретна дейност, изберете я от списъка с **дейности** ; в противен случай всички дейности ще бъдат върнати за избрания потребител.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="2fd7b-111">Имайте предвид, че определени дейности може да не са налични за избор от менюто **дейности** ; обаче тези елементи за проверка ще бъдат върнати, ако са избрани **Покажи резултатите за всички дейности** (настройка по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="2fd7b-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="2fd7b-112">Задайте диапазона от дати и в полето **потребители** изберете потребителското име за потребителя, който искате да изследвате.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="2fd7b-113">Изберете **търсене**.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-113">Select **Search**.</span></span> <span data-ttu-id="2fd7b-114">Дейността се показва под **резултати**.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-114">The activities appear under **Results**.</span></span> <span data-ttu-id="2fd7b-115">Можете да видите IP адреса за всяка дейност.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="2fd7b-116">За да видите подробните данни, изберете дейност и след това изберете **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="2fd7b-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="2fd7b-117">За да научите повече, вижте търсене в [регистрационния файл за проверка на Office 365 за отстраняване на често срещани сценарии](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="2fd7b-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>