---
title: Правила за споделяне на календар в 618
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684219"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Грешка в правилата при споделяне на календар

1. Направете едно от следните неща, както е подходящо за вашата ситуация:
    - Свържете се с Exchange Online, като използвате отдалечен PowerShell. За повече информация вижте [Свързване към Exchange Online чрез отдалечен PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - В локалния сървър Отворете обвивката за управление на Exchange.
2. Определяне на правилата за споделяне, присвоени на потребителя. За да направите това, изпълнете следната команда и имайте предвид, че върнатите правила:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Актуализиране на правилата за споделяне за потребителя. За да направите това, изпълнете следните стъпки:
    - Отворете центъра за администриране на Exchange.
    - Щракнете върху **организация**и след това щракнете двукратно върху правилото, което е присвоено на потребителя под **индивидуално споделяне**. Това е правилото, което е върнато в стъпка 2.
    - На страницата правило за споделяне изберете ниво на споделяне на календара, което искате да разрешите под **Задаване каква информация искате да споделите**; щракнете върху **Запиши**.

За повече информация вижте: ["правилата не позволяват даване на разрешения на това ниво на една или повече от тези получатели", когато потребителят се опитва да сподели календар](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
