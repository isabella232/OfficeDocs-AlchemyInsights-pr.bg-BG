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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672422"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix проблеми с доставка за код на грешка 550

Този проблем възниква [, когато проверявате дали имейл адрес е валиден за предотвратяване на премии](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Office 365. Опитайте следното:

1. Определете дали проблемът е специфичен за целия домейн или един имейл адрес:
    - Целия домейн: понякога домейна трябва да бъде синхронизиран; Опитайте да [зададете домейн вътрешен и след това обратно към авторитетен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Единичен имейл адрес: понякога адресът трябва да бъде синхронизиран; промяна на SMTP прокси адрес и след това да го промените обратно може да помогне.
2. Определете дали проблемът е специфичен за група или публична папка. За някои типове обекти може да се наложи да бъдат създадени ръчно в Azure Active Directory.

Ако имате нужда от допълнителна помощ, моля, отворете билет за поддръжка и укажете обхвата на проблема (включително типа на обекта, който изпращате), за да можем да ви съдействаме по-добре.