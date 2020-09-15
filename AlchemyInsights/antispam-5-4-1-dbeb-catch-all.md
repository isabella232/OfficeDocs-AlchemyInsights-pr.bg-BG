---
title: Антиспам DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717350"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="c593e-102">Отстраняване на проблеми с доставянето на код на грешка 550 5.4.1 Relay отказан достъп</span><span class="sxs-lookup"><span data-stu-id="c593e-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="c593e-103">Този проблем възниква при [проверка дали имейл адресът е валиден за предотвратяване на bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c593e-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="c593e-104">Изпробвайте следното:</span><span class="sxs-lookup"><span data-stu-id="c593e-104">Try the following:</span></span>

1. <span data-ttu-id="c593e-105">Определяне дали проблемът е специфичен за цял домейн, или за един имейл адрес:</span><span class="sxs-lookup"><span data-stu-id="c593e-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="c593e-106">Целият домейн: понякога домейнът трябва да бъде синхронизиран; Опитайте да [зададете домейна на вътрешен и след това да се върнете към достоверен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="c593e-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="c593e-107">Отделен имейл адрес: понякога адресът трябва да бъде синхронизиран; промяна на адреса на SMTP прокси сървър и след това смяната му може да ви помогне.</span><span class="sxs-lookup"><span data-stu-id="c593e-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="c593e-108">Определяне дали проблемът е конкретен за група или за публична папка.</span><span class="sxs-lookup"><span data-stu-id="c593e-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="c593e-109">За някои типове обекти може да се наложи обектите да бъдат ръчно създадени в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c593e-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="c593e-110">Ако имате нужда от допълнителна помощ, отворете билет за поддръжка и задайте обхвата на проблема (включително типа на обекта, който изпращате), така че да можем да ви помогнем по-добре.</span><span class="sxs-lookup"><span data-stu-id="c593e-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>