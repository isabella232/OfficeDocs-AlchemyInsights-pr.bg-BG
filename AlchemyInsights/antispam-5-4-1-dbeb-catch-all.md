---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821436"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="031eb-102">Коригиране на проблеми с доставянето за код на грешка 550 5.4.1 Предаване на достъпа е отказан</span><span class="sxs-lookup"><span data-stu-id="031eb-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="031eb-103">Този проблем възниква, [когато проверявате дали имейл адресът е валиден, за да предотвратите отпадания](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="031eb-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="031eb-104">Опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="031eb-104">Try the following:</span></span>

1. <span data-ttu-id="031eb-105">Определете дали проблемът е специфичен за цял домейн, или за един имейл адрес:</span><span class="sxs-lookup"><span data-stu-id="031eb-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="031eb-106">Цял домейн: Понякога домейнът трябва да бъде синхронизиран; опитайте [да зададете домейна на "Вътрешен" и след това да се върнете към "Авторитет".](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="031eb-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="031eb-107">Един имейл адрес: Понякога адресът трябва да бъде синхронизиран; промяната на адреса на smtp прокси сървъра и след това промяната му обратно може да помогне.</span><span class="sxs-lookup"><span data-stu-id="031eb-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="031eb-108">Определете дали проблемът е специфичен за група, или за публична папка.</span><span class="sxs-lookup"><span data-stu-id="031eb-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="031eb-109">За някои типове обекти може да се наложи обектите да се създават ръчно в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="031eb-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="031eb-110">Ако имате нужда от допълнителна помощ, отворете билет за поддръжка и задайте обхвата на проблема (включително типа на обекта, на който изпращате), за да можем да ви помогнем по-добре.</span><span class="sxs-lookup"><span data-stu-id="031eb-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>