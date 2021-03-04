---
title: Намиране на събития, извършени в правила за папка "Входящи"
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429318"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="91ee1-102">Намиране на събития, извършени в правила за папка "Входящи"</span><span class="sxs-lookup"><span data-stu-id="91ee1-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="91ee1-103">Когато се създават, променят или изтриват правила за папка "Входящи", събитията се записват в регистрационния файл за проверка.</span><span class="sxs-lookup"><span data-stu-id="91ee1-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="91ee1-104">Ето как да ги прегледате:</span><span class="sxs-lookup"><span data-stu-id="91ee1-104">Here's how to review them:</span></span>

1. <span data-ttu-id="91ee1-105">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="91ee1-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="91ee1-106">Изберете търсене > на търсене в регистрационния файл за проверка.</span><span class="sxs-lookup"><span data-stu-id="91ee1-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="91ee1-107">Ако видите съобщение, което ви трябва, за да включите проверката, продължете напред и го включете сега.</span><span class="sxs-lookup"><span data-stu-id="91ee1-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="91ee1-108">Ако тази функция не е включена, резултатите от търсенето няма да могат да изтеглят данни от предишни дати.</span><span class="sxs-lookup"><span data-stu-id="91ee1-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="91ee1-109">Изберете полето дейности и намерете дейности на пощенска кутия на Exchange и след това изберете New-InboxRule създаване на правило за папка "Входящи" от Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="91ee1-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="91ee1-110">Когато сте готови, щракнете извън екрана, за да намалите екрана дейности.</span><span class="sxs-lookup"><span data-stu-id="91ee1-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="91ee1-111">Задайте диапазона от дати и след това в полето потребители изберете потребителското име за потребителя, който искате да изследвате.</span><span class="sxs-lookup"><span data-stu-id="91ee1-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="91ee1-112">Можете да изберете повече от един потребител едновременно.</span><span class="sxs-lookup"><span data-stu-id="91ee1-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="91ee1-113">Изберете търсене.</span><span class="sxs-lookup"><span data-stu-id="91ee1-113">Select Search.</span></span> <span data-ttu-id="91ee1-114">Дейността се показва под резултати.</span><span class="sxs-lookup"><span data-stu-id="91ee1-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="91ee1-115">За да видите подробните данни, изберете дейност и след това изберете повече информация.</span><span class="sxs-lookup"><span data-stu-id="91ee1-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="91ee1-116">Под секцията параметри можете да видите името на правилото, набора от условия и действията, които ще предприеме правилото.</span><span class="sxs-lookup"><span data-stu-id="91ee1-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="91ee1-117">За да научите повече, вижте търсене в регистрационния файл за проверка на Office 365 за отстраняване на често срещани сценарии.</span><span class="sxs-lookup"><span data-stu-id="91ee1-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>