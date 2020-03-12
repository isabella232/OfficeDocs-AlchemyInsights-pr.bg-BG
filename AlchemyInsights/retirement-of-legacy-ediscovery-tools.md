---
title: Пенсиониране на наследените инструменти за откриване на електронни данни
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600347"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Пенсиониране на наследените инструменти за откриване на електронни данни

В резултат на новите и подобрени функции за откриване на електронни данни в центъра за съответствие на Microsoft 365, следните стари инструменти и командни елементи ще се оттеглеят през следващите месеци:

- [Откриването на електронни данни](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на място и [задържането на място](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центъра за администриране на Exchange.

- Кратки команди на Exchange Online PowerShell, които поддържат на място eDiscovery и задържа. (Тези кратки команди са общо идентифицирани като *-MailboxSearch кратки команди.) Това включва следните кратки команди:

    - [Търсене на нова пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Търсене на начална пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Търсене на стоп-пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Търсене на set-пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Пощенска [кутия за търсене](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) команда в Exchange Онлайн PowerShell.
- Следните операции в API на уеб услуги на Exchange:
    - [Получаване на пощенски кутии за търсене](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Задаване на пощенски кутии](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Пощенски кутии](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Разширено откриване на електронни данни v1.0 на Office 365](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Времева линия за пенсиониране:**
- 1 април 2020 г.: Няма да можете да създавате нови търсения и задържания, но все още можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск. Поддръжката на Microsoft вече няма да поддържа на място & за откриване на електронни данни в EAC.

- 1 юли 2020 г.: & за откриване на електронни данни на място притежава функции в EAC ще бъдат поставени в режим само за четене. Това означава, че ще можете да премахвате само съществуващи търсения и задържания.

**За повече информация вижте:**

 - [Мигриране на следене на откриването на електронни данни и задържане в центъра за съответствие на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Пенсиониране на наследените инструменти за откриване на електронни данни](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Често задавани въпроси за откриването на електронни данни на място и задържанията на място](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



