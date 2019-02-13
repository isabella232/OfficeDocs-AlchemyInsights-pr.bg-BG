---
title: Преместване на имейл съобщения в архивната пощенска кутия
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941687"
---
Като проблеми, архивиране на елементите в архивната пощенска кутия. Уверете се, че сте извършили следните стъпки:
  
1. Потвърдете, че **Архив пощенска кутия** е разрешен. Ако не, използвайте стъпки в [тази статия](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , за да активирате архивна пощенска кутия. 
    
2. В центъра за администриране на Exchange изберете **Етикети за съхранение** под **Управление на спазването**, създаване на **етикет за съхранение** с действието за **Преместване в Архив** , съдържащ желаните **Задържане на възрастта**.
    
3. В центъра за администриране на Exchange изберете **Правила за задържане**, създаване на **Правила за задържане** и добавете вашето **Преместване в Архив** задържане етикет към тази политика. 
    
4. [Присвояване на правило за](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) конкретна потребителска пощенска кутия. Същата политика ще бъдат приложени към **основната** , така и за **архивната** пощенска кутия. 
    
Пощенската кутия на потребителя трябва да имате архив политика да преместите елементи в архивна пощенска кутия. Тя може да се наложи да принуди управлявана папка помощник (МВНР) да изпълнява и прилага новите настройки за пощенската кутия на потребителя. Изпълнете следната команда докато [свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да започне помощникът за управлявани папки за конкретна пощенска кутия: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Искате ли повече информация за създаване на политика на архив, вижте [Създаване на архив и заличаване правила за пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

