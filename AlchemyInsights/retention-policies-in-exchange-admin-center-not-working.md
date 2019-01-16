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
 <span data-ttu-id="047d6-102">**Изход:** Новосъздадени или актуализирани задържане политика в центъра за администриране на Exchange не се прилагат за пощенски кутии или са не се премества в архивната пощенска кутия или изтриване на елементи.</span><span class="sxs-lookup"><span data-stu-id="047d6-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="047d6-103">**Основните причини:**</span><span class="sxs-lookup"><span data-stu-id="047d6-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="047d6-p101">Това може да се дължи на **Помощникът за управлявани папки** не е обработен на потребителската пощенска кутия. Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия в облака организация веднъж на всеки седем дни. Ако промените етикет за съхранение или приложите различни правила за съхранение към пощенска кутия, можете да изчакате докато управлява папка подпомагат обработва пощенската кутия, или можете да стартирате Start-ManagedFolderAssistant cmdlet да започне помощникът за управлявани папки да обработи конкретен пощенска кутия. Работещи тази кратка команда е полезна за тестване или отстраняване на политика на задържане или задържане етикет настройки. За повече информация посетете [тичам помощникът за управлявани папки](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="047d6-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="047d6-109">**Разтвор:** Изпълнете следната команда да започне помощникът за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="047d6-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="047d6-p102">Това може да възникне и ако **RetentionHold** е било **разрешено** на пощенската кутия. Ако пощенската кутия е бил поставен на RetentionHold, правилото за съхранение за пощенската кутия няма да бъдат обработвани по това време. За повече информация относно настройката вижте RetentionHold: [Пощенска кутия задържане](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="047d6-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="047d6-113">**Решение:**</span><span class="sxs-lookup"><span data-stu-id="047d6-113">**Solution:**</span></span>
    
  - <span data-ttu-id="047d6-114">Проверка на състоянието на настройката на RetentionHold на конкретна пощенска кутия в [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="047d6-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="047d6-115">Изпълнете следната команда да **забраните** RetentionHold определена пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="047d6-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="047d6-116">Сега изпълнете отново папката управлявани помощник:</span><span class="sxs-lookup"><span data-stu-id="047d6-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="047d6-117">**Забележка:** Ако пощенската кутия е по-малък от 10 MB, помощникът за управлявани папки ще не автоматично обработва пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="047d6-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

