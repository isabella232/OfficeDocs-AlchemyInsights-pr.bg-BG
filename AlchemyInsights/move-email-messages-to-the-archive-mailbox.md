---
title: Преместване на имейл съобщения в пощенската кутия "Архив"
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974946"
---
# <a name="move-email-to-the-archive-mailbox"></a>Преместване на имейл в архивната пощенска кутия

Ако искате да изпълняваме автоматизирани проверки за настройките, споменати по-долу, изберете бутона назад < – в горната част на тази страница и след това въведете имейл адреса на потребителя, който има проблеми с преместването на имейла в архивната си пощенска кутия.

1. Уверете се, че **е разрешена пощенска** кутия за архивиране. Ако не, използвайте стъпките в тази [статия, за да](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) разрешите архивната пощенска кутия.

2. За да архивирате автоматично съобщенията в архивната пощенска кутия, етикет за съхранение с действието Преместване в архива трябва да бъде настроен да се прилага автоматично към цялата пощенска кутия **(по подразбиране).**  Използвайте стъпките тук, за да създадете етикета: Етикет ["Архив по подразбиране".](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. След това добавете **етикета Архив** към правилата си за съхранение. В центъра Exchange за администриране изберете Правила за **съхранение,** > да добавите етикета Преместване в архива към правилата > **Запиши**. 

4. Сега [задайте правилата за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) на пощенската кутия на конкретен потребител. Едни и същи правила ще бъдат приложени както към основната, **така и** към пощенската кутия **"Архив".**

Може да се наложи да накарате помощника за управлявани папки (MFA) да изпълнява и прилага новите настройки към пощенската кутия на потребителя. Изпълнете следната команда, докато [сте свързани към EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) за да стартирате помощника за управлявани папки за определена пощенска кутия:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване за пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  