---
title: Разберете кой е настроил препращането на пощенска кутия и как
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481019"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="bd415-102">Разберете кой е настроил препращането на пощенска кутия и как</span><span class="sxs-lookup"><span data-stu-id="bd415-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="bd415-103">Ако е зададена външна препращане в пощенска кутия, дейността се проверява като част от кратката команда за Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="bd415-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="bd415-104">Ето как да намерите дейността в регистрационния файл за проверка:</span><span class="sxs-lookup"><span data-stu-id="bd415-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="bd415-105">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="bd415-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="bd415-106">Изберете **търсене** в >  **регистрационния файл за проверка**.</span><span class="sxs-lookup"><span data-stu-id="bd415-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="bd415-107">Ако видите съобщение, което ви трябва, за да включите проверката, продължете напред и го включете сега.</span><span class="sxs-lookup"><span data-stu-id="bd415-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="bd415-108">Ако тази функция не е включена, резултатите от търсенето няма да могат да изтеглят данни от предишни дати.</span><span class="sxs-lookup"><span data-stu-id="bd415-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="bd415-109">Уверете се, че полето **дейности** е настроено да **показва резултати за всички дейности** (по подразбиране).</span><span class="sxs-lookup"><span data-stu-id="bd415-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="bd415-110">Задайте диапазона от дати.</span><span class="sxs-lookup"><span data-stu-id="bd415-110">Specify the date range.</span></span> <span data-ttu-id="bd415-111">Не е нужно да указвате потребителско име.</span><span class="sxs-lookup"><span data-stu-id="bd415-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="bd415-112">Изберете **търсене**.</span><span class="sxs-lookup"><span data-stu-id="bd415-112">Select **Search**.</span></span> <span data-ttu-id="bd415-113">Дейността се показва под **резултати**.</span><span class="sxs-lookup"><span data-stu-id="bd415-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="bd415-114">Изберете **филтриране на резултатите**, след което въведете **Set-пощенска кутия** в полето Филтър за **дейност** .</span><span class="sxs-lookup"><span data-stu-id="bd415-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="bd415-115">Това връща всички дейности за **зададена пощенска кутия** .</span><span class="sxs-lookup"><span data-stu-id="bd415-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="bd415-116">За да прегледате подробностите, изберете дейност и след това изберете **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="bd415-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="bd415-117">Под **параметри** можете да видите препращане на имейл адреса, който е зададен в пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="bd415-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="bd415-118">**Потребителското име** представлява потребителя, който е настроил външно препращане в пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="bd415-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="bd415-119">За да научите повече, вижте [търсене в регистрационния файл за проверка на Office 365 за отстраняване на често срещани сценарии](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="bd415-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>