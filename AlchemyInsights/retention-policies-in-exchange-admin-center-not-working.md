---
title: Правилата за съхранение в центъра за администриране на Exchange не работят
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740499"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Правила за съхранение в центъра за администриране на Exchange

Ако искате да изпълняваме автоматизирани проверки за настройките, упоменати по-долу, изберете бутона Назад < – в горния край на тази страница и след това въведете имейл адреса на потребителя, който има проблеми с правилата за съхранение.

 **Проблем:** Новосъздадените или актуализираните правила за съхранение в центъра за администриране на Exchange не се прилагат към пощенските кутии или елементите не се преместват в пощенската кутия или изтриват. 
  
 **Главни причини:**
  
- Това може да се дължи на факта, че **Помощникът за управление на папки** не е обработил пощенската кутия на потребителя. Помощникът за управление на папки се опитва да обработи всяка пощенска кутия във вашата организация, базирана на облак, на всеки седем дни. Ако промените етикет за съхранение или прилагате други правила за съхранение към пощенска кутия, можете да изчакате, докато управляваната папка помогне за процеса на пощенската кутия, или можете да изпълните кратката команда Start-ManagedFolderAssistant, за да стартирате помощника за управление на папки, за да обработите конкретна пощенска кутия. Изпълнението на тази кратка команда е полезно за тестване или отстраняване на неизправности при правила за съхранение или настройки на етикети за съхранение. За повече информация посетете [изпълнение на помощника за управление на папки](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Решение:** Изпълнете следната команда, за да стартирате помощника за управление на папки за конкретна пощенска кутия:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Това може да се случи и ако **RetentionHold** е **разрешена** за пощенската кутия. Ако пощенската кутия е поставена върху RetentionHold, правилата за съхранение в пощенската кутия няма да бъдат обработени през това време. За повече инсталациите в настройката за RetentionHold вижте: [задържане на съхранение на пощенска кутия](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Решение**
    
  - Проверете състоянието на настройката RetentionHold на конкретната пощенска кутия в [ЕКСО PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Изпълнете следната команда, за да **забраните** RetentionHold в конкретна пощенска кутия:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Сега стартирайте повторно помощника за управление на папки:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Забележка:** Ако една пощенска кутия е по-малка от 10 МБ, помощникът за управление на папки няма да обработва автоматично пощенската кутия.
 
За повече информация относно правилата за съхранение в центъра за администриране на Exchange вижте:
- [Етикети за съхранение и правила за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Прилагане на правила за съхранение към пощенски кутии](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Добавяне или премахване на етикети за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Как да идентифицирате типа на задържане, поставен върху пощенска кутия](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
