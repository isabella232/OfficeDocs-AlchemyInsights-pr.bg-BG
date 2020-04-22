---
title: Преместване на имейл съобщения в архивнапощенска кутия
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713635"
---
# <a name="move-email-to-the-archive-mailbox"></a>Преместване на имейл а в архивната пощенска кутия

1. Уверете се, че **архивнапощенска кутия** е разрешена. Ако не, използвайте стъпките в [тази статия,](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) за да разрешите архивна пощенска кутия.

2. За да архивирате автоматично съобщения тава архивната пощенска кутия, етикет за задържане с **действие "Преместване в архив"** трябва да бъде зададен на **автоматично приложение към цялата пощенска кутия (по подразбиране) етикет**. Използвайте стъпките тук, за да създадете маркера: [Архив по подразбиране таг](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. След това добавете **етикета "Архив"** към правилата за задържане. В центъра за администриране на Exchange изберете **Правила за задържане** > добавите етикет **"Преместване в архив"** към правилата > **Записване**.

4. Сега [присвоите правило](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за пощенска кутия на конкретен потребител. Същата политика ще се прилагат за **основните** и **архивната** пощенска кутия.

Може да е необходимо да накарате помощника управлявани папки (МВНР) да изпълни и приложи новите настройки на пощенската кутия на потребителя. Изпълнете следната команда, докато [е свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:
  
Асистент за начало на управлявани папки -самоличност<name of the mailbox>

За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  