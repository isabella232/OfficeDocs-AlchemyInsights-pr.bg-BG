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
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418277"
---
# <a name="move-email-to-the-archive-mailbox"></a>Премести имейл в архивната пощенска кутия
 
1. Потвърдете, че **Архив пощенска кутия** е разрешен. Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) за да активирате архивна пощенска кутия.

2. За да архивирате съобщения автоматично в архивната пощенска кутия, етикет за съхранение с действието за **Преместване в Архив** трябва да се настрои да **прилага автоматично за целия пощенска кутия (по подразбиране) етикет**. Използвайте стъпки тук, за да създадете етикет: [Архив по подразбиране етикет](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. След това добавете **Архив** етикет към вашите правила за задържане. В центъра за администриране на Exchange изберете **Правила за задържане** > добави **Премести в Архив етикет** към политиката > **записване**. 
    
4. Сега [присвоите правило за](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) конкретна потребителска пощенска кутия. Същата политика ще бъдат приложени към **основната** , така и за **архивната** пощенска кутия. 
    
Тя може да се наложи да принуди управлявана папка помощник (МВНР) да изпълнява и прилага новите настройки за пощенската кутия на потребителя. Изпълнете следната команда докато [свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да започне помощникът за управлявани папки за конкретна пощенска кутия: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

За повече информация относно настройването на политика на Архив вижте [Създаване на архив и заличаване правила за пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

