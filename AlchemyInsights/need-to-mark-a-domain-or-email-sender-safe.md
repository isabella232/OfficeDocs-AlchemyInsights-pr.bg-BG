---
title: Трябва да маркирате домейн или имейл подател безопасно?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281119"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="66789-102">Трябва да маркирате домейн или имейл подател безопасно?</span><span class="sxs-lookup"><span data-stu-id="66789-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="66789-103">Не се препоръчва използването на **списъци с безопасни податели,** тъй като тя отваря вашата организация за нежелана, фиш и подправяне на атаки.</span><span class="sxs-lookup"><span data-stu-id="66789-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="66789-104">Ако обаче има бизнес изискване, **препоръчваме да** използвате за това **[правилата за пощенски поток.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="66789-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="66789-105">Нашите указания гарантират удостоверяване на изпращача (проверява изпращане на домейн не се подмества).</span><span class="sxs-lookup"><span data-stu-id="66789-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="66789-106">**Забележка:** Не препоръчваме да управлявате фалшиви положителни резултати чрез списъци на безопасни податели, защото изключенията при филтрирането на нежелана информация могат да отворят организацията ви за атаки на защитата.</span><span class="sxs-lookup"><span data-stu-id="66789-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="66789-107">Ако вашите потребители получават съобщения, неправилно маркирани като спам или нежелана поща, **[моля, изпратете съобщение до Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="66789-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="66789-108">Безопасните податели в Outlook, разрешен списък с податели или разрешен списък с домейни в анти-спам политики **трябва да се избягва,** защото подателите заобикалят всички спам, измамни и фиш защита и удостоверяване на подателя (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="66789-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="66789-109">Този метод се използва най-добре само за временно тестване.</span><span class="sxs-lookup"><span data-stu-id="66789-109">This method is best used for temporary testing only.</span></span>
