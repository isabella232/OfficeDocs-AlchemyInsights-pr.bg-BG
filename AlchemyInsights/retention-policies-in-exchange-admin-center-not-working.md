---
title: Правила за съхранение в центъра за администриране на Exchange не работи
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551332"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Правила за съхранение в центъра за администриране на Exchange

 **Изход:** Новосъздадени или актуализирани задържане политика в центъра за администриране на Exchange не се прилагат за пощенски кутии или са не се премества в архивната пощенска кутия или изтриване на елементи. 
  
 **Основните причини:**
  
- Това може да се дължи на **Помощникът за управлявани папки** не е обработен на потребителската пощенска кутия. Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия в облака организация веднъж на всеки седем дни. Ако промените етикет за съхранение или приложите различни правила за съхранение към пощенска кутия, можете да изчакате докато управлява папка подпомагат обработва пощенската кутия, или можете да стартирате Start-ManagedFolderAssistant cmdlet да започне помощникът за управлявани папки да обработи конкретен пощенска кутия. Работещи тази кратка команда е полезна за тестване или отстраняване на политика на задържане или задържане етикет настройки. За повече информация посетете [тичам помощникът за управлявани папки](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Разтвор:** Изпълнете следната команда да започне помощникът за управлявани папки за конкретна пощенска кутия:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Това може да възникне и ако **RetentionHold** е било **разрешено** на пощенската кутия. Ако пощенската кутия е бил поставен на RetentionHold, правилото за съхранение за пощенската кутия няма да бъдат обработвани по това време. За повече информация относно настройката вижте RetentionHold: [Пощенска кутия задържане](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Решение:**
    
  - Проверка на състоянието на настройката на RetentionHold на конкретна пощенска кутия в [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Изпълнете следната команда да **забраните** RetentionHold определена пощенска кутия:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Сега изпълнете отново папката управлявани помощник:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Забележка:** Ако пощенската кутия е по-малък от 10 MB, помощникът за управлявани папки ще не автоматично обработва пощенската кутия.
 
За повече информация за правила за съхранение в центъра за администриране на Exchange вижте:
- [Етикетите и задържане полиция](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Прилагане на правила за задържане към пощенски кутии](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Добавяне или премахване на етикети за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Как да се идентифицират типа на задържане пуснати на пощенска кутия](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
