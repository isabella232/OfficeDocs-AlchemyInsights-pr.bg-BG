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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Отстраняване на проблеми с доставянето на код на грешка 550 5.4.1 Relay отказан достъп

Този проблем възниква при [проверка дали имейл адресът е валиден за предотвратяване на bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft. Изпробвайте следното:

1. Определяне дали проблемът е специфичен за цял домейн, или за един имейл адрес:
    - Целият домейн: понякога домейнът трябва да бъде синхронизиран; Опитайте да [зададете домейна на вътрешен и след това да се върнете към достоверен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Отделен имейл адрес: понякога адресът трябва да бъде синхронизиран; промяна на адреса на SMTP прокси сървър и след това смяната му може да ви помогне.
2. Определяне дали проблемът е конкретен за група или за публична папка. За някои типове обекти може да се наложи обектите да бъдат ръчно създадени в Azure Active Directory.

Ако имате нужда от допълнителна помощ, отворете билет за поддръжка и задайте обхвата на проблема (включително типа на обекта, който изпращате), така че да можем да ви помогнем по-добре.