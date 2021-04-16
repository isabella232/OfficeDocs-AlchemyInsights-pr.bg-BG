---
title: Трябва да маркирате домейн или имейл подател в безопасност?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792121"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="e4a53-102">Трябва да маркирате домейн или имейл подател в безопасност?</span><span class="sxs-lookup"><span data-stu-id="e4a53-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="e4a53-103">Използването на **списъци с безопасни податели не** се препоръчва, тъй като отваря вашата организация за нежелана поща, фишинг и измамни атаки.</span><span class="sxs-lookup"><span data-stu-id="e4a53-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="e4a53-104">Ако обаче има бизнес изискване, ви препоръчваме да използвате **правила** за **[пощенски поток](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** за това.</span><span class="sxs-lookup"><span data-stu-id="e4a53-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="e4a53-105">Нашите указания гарантират удостоверяване на подателя (проверява, че домейнът за изпращане не се подпрагва).</span><span class="sxs-lookup"><span data-stu-id="e4a53-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="e4a53-106">**Забележка:** Не препоръчваме да управлявате грешни положителни резултати с помощта на списъци с безопасни податели, тъй като изключенията от филтрирането на нежелана поща могат да отворят вашата организация за атаки на защитата.</span><span class="sxs-lookup"><span data-stu-id="e4a53-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="e4a53-107">Ако вашите потребители получават съобщения, неправилно маркирани като нежелана поща или нежелана поща, **[докладвайте за съобщения и файлове на Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="e4a53-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="e4a53-108">Безопасните податели в Outlook, списъка с разрешени податели или разрешените домейни в правилата за нежелана поща трябва да се избягват, защото подателите заобикалят всички нежелана поща, подлост и фиш защита и удостоверяване на подателя (SPF, DKIM, DMARC). </span><span class="sxs-lookup"><span data-stu-id="e4a53-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="e4a53-109">Този метод се използва най-добре само за временно тестване.</span><span class="sxs-lookup"><span data-stu-id="e4a53-109">This method is best used for temporary testing only.</span></span>
