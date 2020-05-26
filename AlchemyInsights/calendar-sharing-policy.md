---
title: 618 Правила за споделяне на календар
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372988"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Грешка при споделяне на календар

1. Направете едно от следните неща, според вашата ситуация:
    - Свързване с Exchange Online чрез отдалечен PowerShell. За повече информация вижте [Свързване към Exchange Online чрез отдалечен PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - На локалния сървър отворете обвивката на Exchange за управление.
2. Определете правилата за споделяне, които са присвоени на потребителя. За да направите това, изпълнете следната команда и забележете правилата, върнати:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Актуализирайте правилата за споделяне на потребителя. За да направите това, изпълнете следните стъпки:
    - Отворете центъра за администриране на Exchange.
    - Щракнете върху **организация**, след което щракнете двукратно върху правилата, които се присвояват на потребителя в **разделно споделяне**. Това е политиката, която е върната в стъпка 2.
    - На страницата Правило за споделяне изберете нивото на споделяне на календара, което искате да разрешите под **Посочете каква информация искате да споделите;** щракнете върху **Запиши**.

За повече информация вижте: ["Правилата не позволяват предоставяне то разрешения на това ниво на един или повече от получателите" грешка при опит за споделяне на календар](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
