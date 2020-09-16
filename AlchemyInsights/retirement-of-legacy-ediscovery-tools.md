---
title: Оттегляне на стари инструменти за откриване на електронни данни
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727772"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Оттегляне на стари инструменти за откриване на електронни данни

Като резултат от новата и усъвършенстваната функционалност на откриването на електронни данни в центъра за съответствие на Microsoft 365, следните инструменти за откриване на електронни данни и кратки команди ще бъдат оттеглени през следващите месеци:

- [Откриване](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на електронни данни и [задържане](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) на места в центъра за администриране на Exchange.

- Кратките команди на PowerShell на Exchange Online, които поддържат откриването на електронни данни и задържане на места. (Тези кратки команди се идентифицират общо като *-MailboxSearch кратки команди.) Това включва следните кратки команди:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Стоп-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Кратката команда [търсене – пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.
- Следните операции в API на уеб услугите на Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Разширено откриване на електронни данни v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Времева линия за пенсиониране**:
- **1 юли 2020 г.** Вече не можете да създавате нови търсения и трюмове, но можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск. Поддръжката на Microsoft вече не поддържа откриване на електронни данни на места & съдържа в EAC.
    
- **1 октомври 2020 г.** Откриване на електронни данни на място & съдържа функционалност в EAC ще бъдат поставени в режим само за четене, така че да можете да премахвате съществуващите търсения и съдържания.

**За повече информация вижте**:

 - [Мигриране на стари търсения на откриване на електронни данни и задържане в центъра за съответствие на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Оттегляне на стари инструменти за откриване на електронни данни](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [ЧЗВ за откриване на електронни данни на места и задържане на места](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



