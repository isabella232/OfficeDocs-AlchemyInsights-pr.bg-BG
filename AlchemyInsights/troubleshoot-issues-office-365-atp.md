---
title: Отстраняване на проблеми с Microsoft Defender за Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801396"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="fe436-102">Отстраняване на проблеми с Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="fe436-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="fe436-103">**Забелязвате ли закъснения с доставянето на имейл съобщения** ?</span><span class="sxs-lookup"><span data-stu-id="fe436-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="fe436-104">Опитайте да използвате опцията за динамично доставяне за вашите правила за безопасни прикачени файлове за ATP.</span><span class="sxs-lookup"><span data-stu-id="fe436-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="fe436-105">Това ще предотврати закъсненията при доставянето на имейл съобщения, като същевременно защитава получателите от злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="fe436-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="fe436-106">**Искате ли да съобщите за грешни позитиви или фалшиви негативи** ?</span><span class="sxs-lookup"><span data-stu-id="fe436-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="fe436-107">Използвайте тази връзка, за да подадете файла си за анализиране: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="fe436-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="fe436-108">**Знаете ли, че можете да разрешавате защитата от връзки на ATP Safe за имейли, изпратени между хора във вашата организация** ?</span><span class="sxs-lookup"><span data-stu-id="fe436-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="fe436-109">Изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="fe436-109">Follow these steps:</span></span>
    1. <span data-ttu-id="fe436-110">Отидете на https://protection.office.com и влезте.</span><span class="sxs-lookup"><span data-stu-id="fe436-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="fe436-111">Отидете на **Threat management**  >  **Policy**  >  **безопасни връзки** към политиката за управление на заплахите.</span><span class="sxs-lookup"><span data-stu-id="fe436-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="fe436-112">Под **правила, които важат за определени получатели** , редактирайте (или Добавете) политика.</span><span class="sxs-lookup"><span data-stu-id="fe436-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="fe436-113">Изберете **прилагане на безопасни връзки към съобщенията, изпращани в рамките на организацията** .</span><span class="sxs-lookup"><span data-stu-id="fe436-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="fe436-114">Запишете правилата си и позволете около 30 минути, за да могат промените ви да работят по своя начин чрез центъра за изчислителния център.</span><span class="sxs-lookup"><span data-stu-id="fe436-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="fe436-115">За да получите допълнителна помощ за ATP, вижте [Microsoft Defender за Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="fe436-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>