---
title: АнтиСпам 5.4.1 DBEB улов всички
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707900"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="21081-102">Отстраняване на проблеми при доставка за код на грешка 550 5.4.1 реле достъпът отказан</span><span class="sxs-lookup"><span data-stu-id="21081-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="21081-103">Този проблем възниква, когато [проверявате дали имейл адрес е валиден за предотвратяване на отпадане](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="21081-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="21081-104">Опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="21081-104">Try the following:</span></span>

1. <span data-ttu-id="21081-105">Определете дали проблемът е специфичен за цял домейн или един имейл адрес:</span><span class="sxs-lookup"><span data-stu-id="21081-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="21081-106">Целият домейн: Понякога домейнът трябва да бъде синхронизиран; опитайте [да зададете домейна на вътрешен и след това обратно към авторитетен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="21081-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="21081-107">Един имейл адрес: Понякога адресът трябва да бъде синхронизиран; промяна на smtp прокси адреса и след това да го промените обратно може да помогне.</span><span class="sxs-lookup"><span data-stu-id="21081-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="21081-108">Определете дали проблемът е специфичен за група или публична папка.</span><span class="sxs-lookup"><span data-stu-id="21081-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="21081-109">За някои типове обекти може да се наложи да се създаде ръчно обекти в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="21081-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="21081-110">Ако имате нужда от допълнителна помощ, моля, отворете билет за поддръжка и посочете обхвата на проблема (включително вида на обекта, който изпращате), за да можем да ви помогнем по-добре.</span><span class="sxs-lookup"><span data-stu-id="21081-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>