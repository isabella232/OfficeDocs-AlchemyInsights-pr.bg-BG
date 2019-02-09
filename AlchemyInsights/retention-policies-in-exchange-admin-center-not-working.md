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
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786759"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="0fe5d-102">Правила за съхранение в центъра за администриране на Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe5d-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="0fe5d-103">**Изход:** Новосъздадени или актуализирани задържане политика в центъра за администриране на Exchange не се прилагат за пощенски кутии или са не се премества в архивната пощенска кутия или изтриване на елементи.</span><span class="sxs-lookup"><span data-stu-id="0fe5d-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="0fe5d-104">**Основните причини:**</span><span class="sxs-lookup"><span data-stu-id="0fe5d-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="0fe5d-p101">Това може да се дължи на **Помощникът за управлявани папки** не е обработен на потребителската пощенска кутия. Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия в облака организация веднъж на всеки седем дни. Ако промените етикет за съхранение или приложите различни правила за съхранение към пощенска кутия, можете да изчакате докато управлява папка подпомагат обработва пощенската кутия, или можете да стартирате Start-ManagedFolderAssistant cmdlet да започне помощникът за управлявани папки да обработи конкретен пощенска кутия. Работещи тази кратка команда е полезна за тестване или отстраняване на политика на задържане или задържане етикет настройки. За повече информация посетете [тичам помощникът за управлявани папки](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="0fe5d-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="0fe5d-110">**Разтвор:** Изпълнете следната команда да започне помощникът за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="0fe5d-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="0fe5d-p102">Това може да възникне и ако **RetentionHold** е било **разрешено** на пощенската кутия. Ако пощенската кутия е бил поставен на RetentionHold, правилото за съхранение за пощенската кутия няма да бъдат обработвани по това време. За повече информация относно настройката вижте RetentionHold: [Пощенска кутия задържане](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="0fe5d-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="0fe5d-114">**Решение:**</span><span class="sxs-lookup"><span data-stu-id="0fe5d-114">**Solution:**</span></span>
    
  - <span data-ttu-id="0fe5d-115">Проверка на състоянието на настройката на RetentionHold на конкретна пощенска кутия в [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="0fe5d-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="0fe5d-116">Изпълнете следната команда да **забраните** RetentionHold определена пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="0fe5d-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="0fe5d-117">Сега изпълнете отново папката управлявани помощник:</span><span class="sxs-lookup"><span data-stu-id="0fe5d-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="0fe5d-118">**Забележка:** Ако пощенската кутия е по-малък от 10 MB, помощникът за управлявани папки ще не автоматично обработва пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="0fe5d-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

