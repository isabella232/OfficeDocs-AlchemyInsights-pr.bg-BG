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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Отстраняване на проблеми при доставка за код на грешка 550 5.4.1 реле достъпът отказан

Този проблем възниква, когато [проверявате дали имейл адрес е валиден за предотвратяване на отпадане](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft. Опитайте следното:

1. Определете дали проблемът е специфичен за цял домейн или един имейл адрес:
    - Целият домейн: Понякога домейнът трябва да бъде синхронизиран; опитайте [да зададете домейна на вътрешен и след това обратно към авторитетен](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Един имейл адрес: Понякога адресът трябва да бъде синхронизиран; промяна на smtp прокси адреса и след това да го промените обратно може да помогне.
2. Определете дали проблемът е специфичен за група или публична папка. За някои типове обекти може да се наложи да се създаде ръчно обекти в Azure Active Directory.

Ако имате нужда от допълнителна помощ, моля, отворете билет за поддръжка и посочете обхвата на проблема (включително вида на обекта, който изпращате), за да можем да ви помогнем по-добре.