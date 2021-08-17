---
title: Правила за споделяне на календари 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091580"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Грешка в правилата при споделяне на календар

1. Направете едно от следните неща, както е подходящо за вашата ситуация:
    - Свързване да Exchange Online с помощта на Отдалечен PowerShell. За повече информация [вж. Свързване да Exchange Online използване на Отдалечен PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - На локалния сървър отворете обвивката на Exchange за управление.
2. Определете правилата за споделяне, които са присвоени на потребителя. За да направите това, изпълнете следната команда и обърнете внимание на върнатите правила:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Актуализирайте правилата за споделяне за потребителя. За да направите това, изпълнете следните стъпки:
    - Отворете центъра Exchange администриране.
    - Щракнете **върху** Организация и след това щракнете двукратно върху правилата, които са присвоени на потребителя под **Индивидуално споделяне.** Това е правилото, което е върнато в стъпка 2.
    - На страницата Правило за споделяне изберете нивото на споделяне на календара, което искате да разрешите под **Указване на информацията, която искате да споделите;** щракнете **върху Запиши**.

За повече информация вижте: "Правилата не позволяват даване на разрешения на това ниво на една или повече получатели" грешка, когато потребителят се опита [да сподели календара.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
