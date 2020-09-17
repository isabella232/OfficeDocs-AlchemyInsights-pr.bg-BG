---
title: Трябва да маркирате безопасен домейн или имейл подател?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803234"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="b084c-102">Трябва да маркирате безопасен домейн или имейл подател?</span><span class="sxs-lookup"><span data-stu-id="b084c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="b084c-103">Използването на **списъци с безопасни податели не се препоръчва** , тъй като отваря вашата организация за нежелана поща, фишинг и измамнически атаки.</span><span class="sxs-lookup"><span data-stu-id="b084c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="b084c-104">Ако обаче има бизнес изискване, **ви препоръчваме** да използвате правилата за **[пощенския поток](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** за това.</span><span class="sxs-lookup"><span data-stu-id="b084c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="b084c-105">Нашите указания гарантират удостоверяване на подателя (проверява дали изпращането на домейни не е фалшифицирано).</span><span class="sxs-lookup"><span data-stu-id="b084c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="b084c-106">**Забележка**: не препоръчваме управление на неверни положителни резултати с помощта на списъци с безопасни податели, тъй като изключенията за филтриране на нежелана поща могат да отворят вашата организация за атаки по защитата.</span><span class="sxs-lookup"><span data-stu-id="b084c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="b084c-107">Ако вашите потребители получават съобщения, които са неправилно маркирани като спам или нежелана поща, **[съобщете за съобщения и файлове на Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="b084c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="b084c-108">Безопасните податели в Outlook, списъка с разрешени податели или разрешените домейни в правила за нежелана поща **трябва да бъдат избегнати** , тъй като подателите заобикалят всички нежелани съобщения, пародия и защита на подателя и удостоверяването на изпращача (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="b084c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="b084c-109">Този метод се използва най-добре само за временен тест.</span><span class="sxs-lookup"><span data-stu-id="b084c-109">This method is best used for temporary testing only.</span></span>
