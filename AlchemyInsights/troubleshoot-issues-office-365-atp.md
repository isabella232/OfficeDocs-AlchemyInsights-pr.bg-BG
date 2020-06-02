---
title: Отстраняване на проблеми с разширена защита срещу заплахи за Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511101"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="f3c3b-102">Отстраняване на проблеми с Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="f3c3b-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="f3c3b-103">**Забелязвате закъснения с доставка на имейл съобщения?**</span><span class="sxs-lookup"><span data-stu-id="f3c3b-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="f3c3b-104">Опитайте да използвате опцията за динамична доставка за вашите ATP правила за безопасни прикачени файлове.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="f3c3b-105">Това ще предотврати забавянето при доставяне на имейл съобщения, като същевременно защитава получателите от злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="f3c3b-106">**Искате ли да съобщите фалшиви положителни или фалшиви отрицателни резултати?**</span><span class="sxs-lookup"><span data-stu-id="f3c3b-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="f3c3b-107">Използвайте тази връзка, за да изпратите файла си за анализ:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="f3c3b-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="f3c3b-108">**Знаете ли, че можете да активирате защита на ATP Safe Links за имейл, изпратен между хора във вашата организация?**</span><span class="sxs-lookup"><span data-stu-id="f3c3b-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="f3c3b-109">Изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="f3c3b-109">Follow these steps:</span></span>
    1. <span data-ttu-id="f3c3b-110">Отидете в https://protection.office.com и влезте в профила си.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="f3c3b-111">Отидете на Политика за **управление на**  >  **Policy**  >  **заплахите Безопасни връзки**.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="f3c3b-112">Под **Правила, които се прилагат за определени получатели**, редактирайте (или добавете) правила.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="f3c3b-113">Изберете **Прилагане на безопасни връзки към съобщенията, изпратени в рамките на организацията**.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="f3c3b-114">Запазете правилата си и оставете около 30 минути, за да могат промените ви да протечат през център за данни.</span><span class="sxs-lookup"><span data-stu-id="f3c3b-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="f3c3b-115">За да получите допълнителна помощ за ATP, вижте [Разширена защита от заплахи за Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="f3c3b-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>