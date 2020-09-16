---
title: Отстраняване на проблеми с разширените заплахи за защитата на Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758054"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="8cd1c-102">Отстраняване на проблеми с Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="8cd1c-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="8cd1c-103">**Забелязвате ли закъснения с доставянето на имейл съобщения**?</span><span class="sxs-lookup"><span data-stu-id="8cd1c-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="8cd1c-104">Опитайте да използвате опцията за динамично доставяне за вашите правила за безопасни прикачени файлове за ATP.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="8cd1c-105">Това ще предотврати закъсненията при доставянето на имейл съобщения, като същевременно защитава получателите от злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="8cd1c-106">**Искате ли да съобщите за грешни позитиви или фалшиви негативи**?</span><span class="sxs-lookup"><span data-stu-id="8cd1c-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="8cd1c-107">Използвайте тази връзка, за да подадете файла си за анализиране: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="8cd1c-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="8cd1c-108">**Знаете ли, че можете да разрешавате защитата от връзки на ATP Safe за имейли, изпратени между хора във вашата организация**?</span><span class="sxs-lookup"><span data-stu-id="8cd1c-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="8cd1c-109">Изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="8cd1c-109">Follow these steps:</span></span>
    1. <span data-ttu-id="8cd1c-110">Отидете на https://protection.office.com и влезте.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="8cd1c-111">Отидете на **Threat management**  >  **Policy**  >  **безопасни връзки**към политиката за управление на заплахите.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="8cd1c-112">Под **правила, които важат за определени получатели**, редактирайте (или Добавете) политика.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="8cd1c-113">Изберете **прилагане на безопасни връзки към съобщенията, изпращани в рамките на организацията**.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="8cd1c-114">Запишете правилата си и позволете около 30 минути, за да могат промените ви да работят по своя начин чрез центъра за изчислителния център.</span><span class="sxs-lookup"><span data-stu-id="8cd1c-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="8cd1c-115">За да получите допълнителна помощ за ATP, вижте [подобрена защита на заплахи за Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="8cd1c-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>