---
title: Оттегляне на стари инструменти за откриване на електронни данни
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157508"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Оттегляне на стари инструменти за откриване на електронни данни

В резултат на новата и подобрена функционалност за откриване на електронни данни в Центъра за съответствие на Microsoft 365, следните стари инструменти и команди за откриване на електронни данни ще бъдат оттеглени през следващите месеци:

- [Откриване на електронни данни](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на място и [задържане на място](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центъра за администриране на Exchange.

- Кратки команди на Exchange онлайн PowerShell, които поддържат откриване на електронни данни на място и задържане на място. (Тези кратки команди са общо определени като *-MailboxSearch кратки команди.) Това включва следните кратки команди:

    - [Търсене на нова пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Търсене в стартова пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Търсене на пощенски кутии](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Търсене в пощенски кутии](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Кратката команда [за търсене пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange онлайн PowerShell.
- Следните операции в API на уеб услуги на Exchange:
    - [Получаване на пощенски кутии с възможност за търсене](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Вземи пощенски кутии](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 разширено откриване на електронни данни v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Време в пенсия:**
- 1 април 2020 г.: Няма да можете да създавате нови търсения и задържания, но все още можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск. Поддръжката на Microsoft вече няма да поддържа откриване на електронни данни на място & притежава в EAC.

- 1 юли 2020 г.: функцията "откриване на електронни данни на място" & притежава функционалност в EAC ще бъде поставена в режим само за четене. Това означава, че ще можете да премахвате само съществуващи търсения и задържания.

**За повече информация вижте:**

 - [Мигриране на стари eDiscovery търсения и задържа в центъра за съответствие на Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Оттегляне на наследените инструменти за откриване на електронни данни](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Често задавани въпроси за откриване то на място и за задържане на място](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



