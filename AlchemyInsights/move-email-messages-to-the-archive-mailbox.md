---
title: Преместване на имейл съобщения в архивна пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822151"
---
# <a name="move-email-to-the-archive-mailbox"></a>Преместване на имейл в архивна пощенска кутия

1. Потвърдете, че е разрешена **архивна пощенска кутия** . Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , за да разрешите архивна пощенска кутия.

2. За архивиране на съобщения автоматично в архивна пощенска кутия, маркер за задържане с **Преместване за архивиране** на действие трябва да бъде настроен да се **прилага автоматично към цялата пощенска кутия (по подразбиране) етикет**. Използвайте стъпките тук, за да създадете маркера: [архивен маркер по подразбиране](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. След това добавете **Архивният** маркер към правилата си за задържане. В центъра за администриране на Exchange изберете **правила за задържане** > Добавяне на **етикет за преместване на архив** на правилата > **Save**.

4. Сега [присвоите правила за задържане](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) на пощенската кутия на конкретния потребител. Същата политика ще се прилага към **първичната** и **архивната** пощенска кутия.

Може да се наложи да принудите помощника за управлявана папка (МФП) да изпълнява и прилага новите настройки към пощенската кутия на потребителя. Изпълнете следната команда, докато е [свързан към екзо PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:
  
Стартов помощник – самоличност<name of the mailbox>

За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  