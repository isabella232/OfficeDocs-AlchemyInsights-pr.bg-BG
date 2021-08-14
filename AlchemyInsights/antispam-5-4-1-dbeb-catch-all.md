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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932266"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Коригиране на проблеми с доставянето за код на грешка 550 5.4.1 Предаване на достъпа е отказан

Този проблем възниква, [когато проверявате дали имейл адресът е валиден, за да предотвратите отпадания](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при влизане в мрежата на Microsoft. Опитайте следното:

1. Определете дали проблемът е специфичен за цял домейн, или за един имейл адрес:
    - Цял домейн: Понякога домейнът трябва да бъде синхронизиран; опитайте [да зададете домейна на "Вътрешен" и след това да се върнете към "Авторитет".](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Един имейл адрес: Понякога адресът трябва да бъде синхронизиран; промяната на адреса на smtp прокси сървъра и след това промяната му обратно може да помогне.
2. Определете дали проблемът е специфичен за група, или за публична папка. За някои типове обекти може да се наложи обектите да се създават ръчно в Azure Active Directory.

Ако имате нужда от допълнителна помощ, отворете билет за поддръжка и задайте обхвата на проблема (включително типа на обекта, на който изпращате), за да можем да ви помогнем по-добре.