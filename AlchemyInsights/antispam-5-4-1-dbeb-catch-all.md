---
title: Антиспам ДБЕБ улов-всички
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964057"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f3940-102">Fix проблеми с доставка за код на грешка 550</span><span class="sxs-lookup"><span data-stu-id="f3940-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f3940-103">Този проблем възниква [, когато проверявате дали имейл адрес е валиден за предотвратяване на премии](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Office 365.</span><span class="sxs-lookup"><span data-stu-id="f3940-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="f3940-104">Опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="f3940-104">Try the following:</span></span>

1. <span data-ttu-id="f3940-105">Определете дали проблемът е специфичен за целия домейн или един имейл адрес:</span><span class="sxs-lookup"><span data-stu-id="f3940-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f3940-106">Целия домейн: понякога домейна трябва да бъде синхронизиран; Опитайте да [зададете домейн вътрешен и след това обратно към авторитетен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="f3940-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="f3940-107">Единичен имейл адрес: понякога адресът трябва да бъде синхронизиран; промяна на SMTP прокси адрес и след това да го промените обратно може да помогне.</span><span class="sxs-lookup"><span data-stu-id="f3940-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f3940-108">Определете дали проблемът е специфичен за група или публична папка.</span><span class="sxs-lookup"><span data-stu-id="f3940-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f3940-109">За някои типове обекти може да се наложи да бъдат създадени ръчно в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3940-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f3940-110">Ако имате нужда от допълнителна помощ, моля, отворете билет за поддръжка и укажете обхвата на проблема (включително типа на обекта, който изпращате), за да можем да ви съдействаме по-добре.</span><span class="sxs-lookup"><span data-stu-id="f3940-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>