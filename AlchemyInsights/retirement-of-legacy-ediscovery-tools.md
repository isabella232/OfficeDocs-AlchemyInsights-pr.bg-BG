---
title: Оттегляне на наследените инструменти за откриване на електронни данни
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
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074635"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Оттегляне на наследените инструменти за откриване на електронни данни

В резултат на новата и подобрена функционалност за откриване на електронни данни в центъра за съответствие на Microsoft 365, следните стари инструменти и командни команди за откриване на електронни данни ще бъдат оттеглени през следващите месеци:

- [Откриване на електронни данни на](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) място и задържане на място [в](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) центъра за администриране Exchange място.

- Кратките команди Exchange Online PowerShell, които поддържат In-Place откриване на електронни In-Place задържане. (Тези кратки команди се идентифицират колективно като кратки команди *-MailboxSearch.) Това включва следните кратки команди:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Кратката [команда "Пощенска](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) кутия за търсене" в Exchange Online PowerShell.
- Следните операции в API на Exchange уеб услуги:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Времева линия за пенсиониране:**
- **1 юли 2020 г.** Вече не можете да създавате нови търсения и задържания, но можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск. Поддръжката на Microsoft вече не In-Place откриване на електронни данни & задържа в EAC.
    
- **1 октомври 2020** г. In-Place откриване на електронни данни & Има функционалност в EAC ще бъде поставена в режим само за четене, така че можете да премахвате само съществуващи търсения и задържания.

**За повече информация вижте**:

 - [Мигриране на стари търсения за откриване на електронни Център за съответствие на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Оттегляне на стари инструменти за откриване на електронни данни](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Често задавани въпроси за In-Place откриване на електронни и In-Place задържания](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



