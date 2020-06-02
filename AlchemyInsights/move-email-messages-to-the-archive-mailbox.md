---
title: Преместване на имейл съобщения в архивната пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511029"
---
# <a name="move-email-to-the-archive-mailbox"></a>Преместване на имейл в архивната пощенска кутия

1. Потвърдете, че **архивна пощенска кутия** е разрешена. Ако не, използвайте стъпките в [тази статия,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) за да разрешите архивна пощенска кутия.

2. За да архивирате съобщенията автоматично в архивната пощенска кутия, трябва да бъде зададен маркер за задържане с действието **Преместване в архива,** който се **прилага автоматично към етикета на цялата пощенска кутия (по подразбиране)**. Използвайте стъпките тук, за да създадете етикета: [Архив подразбиращ се етикет](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. След това добавете етикета **"Архив"** към правилата си за задържане. В центъра за администриране на Exchange изберете **Правила за задържане** > добавите **етикета Премести в архива** към правилата > **Записване**.

4. Сега [присвоите правило](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за съхранение на пощенска кутия на конкретен потребител. Същите правила ще се прилагат към **първична** и **архивна** пощенска кутия.

Може да се наложи да накарате помощника за управлявани папки (МРН) да стартирате и приложите новите настройки на пощенската кутия на потребителя. Изпълнете следната команда, докато [е свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:
  
Начален управляемпаксовразставник -идентичност<name of the mailbox>

За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  