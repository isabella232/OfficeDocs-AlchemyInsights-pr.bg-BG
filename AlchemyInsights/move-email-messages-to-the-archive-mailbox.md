---
title: Местене на имейл съобщения в архивната пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799769"
---
# <a name="move-email-to-the-archive-mailbox"></a>Преминаване на имейл в пощенската кутия за архивиране

Ако искате да изпълняваме автоматизирани проверки за настройките, упоменати по-долу, изберете бутона "назад" < – в горния край на тази страница и след това въведете имейл адреса на потребителя, който има проблеми при преместване на имейла в своята архивна пощенска кутия.

1. Проверете дали е разрешена **пощенска кутия за архивиране** . Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , за да разрешите архивната пощенска кутия.

2. За да архивирате съобщения автоматично в архивната пощенска кутия, трябва да се настрои етикет за съхранение с действието **за преминаване към архивиране** , за да се **Приложи автоматично към етикета на цялата пощенска кутия (по подразбиране)**. Използвайте стъпките тук, за да създадете етикет: [Архивирай етикета по подразбиране](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. След това добавете етикета за **архивиране** към правилата за съхранение. В центъра за администриране на Exchange изберете **правила за съхранение** > Добавете **етикета преминаване към архивиране** към правилата > **Запиши**.

4. Сега [Задайте правилата за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за конкретната пощенска кутия на потребителя. Същите правила ще бъдат прилагани както за **първичната** , така и за **архивната** пощенска кутия.

Може да се наложи да принудите помощника за управление на папки (МВНР) да изпълнява и да прилага новите настройки към пощенската кутия на потребителя. Изпълнете следната команда, докато [сте свързани към ЕКСО PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , за да стартирате помощника за управление на папки за конкретна пощенска кутия:
  
Start-ManagedFolderAssistant-самоличност <name of the mailbox>

За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване за пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  