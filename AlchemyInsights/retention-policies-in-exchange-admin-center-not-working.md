---
title: Правила за съхранение в центъра за администриране на Exchange не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275609"
---
 **Изход:** Новосъздадени или актуализирани задържане политика в центъра за администриране на Exchange не се прилагат за пощенски кутии или са не се премества в архивната пощенска кутия или изтриване на елементи. 
  
 **Основните причини:**
  
- Това може да се дължи на **Помощникът за управлявани папки** не е обработен на потребителската пощенска кутия. Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия в облака организация веднъж на всеки седем дни. Ако промените етикет за съхранение или приложите различни правила за съхранение към пощенска кутия, можете да изчакате докато управлява папка подпомагат обработва пощенската кутия, или можете да стартирате Start-ManagedFolderAssistant cmdlet да започне помощникът за управлявани папки да обработи конкретен пощенска кутия. Работещи тази кратка команда е полезна за тестване или отстраняване на политика на задържане или задържане етикет настройки. За повече информация посетете [тичам помощникът за управлявани папки](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Разтвор:** Изпълнете следната команда да започне помощникът за управлявани папки за конкретна пощенска кутия: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Това може да възникне и ако **RetentionHold** е било **разрешено** на пощенската кутия. Ако пощенската кутия е бил поставен на RetentionHold, правилото за съхранение за пощенската кутия няма да бъдат обработвани по това време. За повече информация относно настройката вижте RetentionHold: [Пощенска кутия задържане](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Решение:**
    
  - Проверка на състоянието на настройката на RetentionHold на конкретна пощенска кутия в [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
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
  

