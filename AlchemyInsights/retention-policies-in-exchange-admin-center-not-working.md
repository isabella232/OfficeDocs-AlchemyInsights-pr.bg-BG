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
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369654"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="14fe1-102">Правила за съхранение в центъра за администриране на Exchange</span><span class="sxs-lookup"><span data-stu-id="14fe1-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="14fe1-103">**Изход:** Новосъздадени или актуализирани задържане политика в центъра за администриране на Exchange не се прилагат за пощенски кутии или са не се премества в архивната пощенска кутия или изтриване на елементи.</span><span class="sxs-lookup"><span data-stu-id="14fe1-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="14fe1-104">**Основните причини:**</span><span class="sxs-lookup"><span data-stu-id="14fe1-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="14fe1-105">Това може да се дължи на **Помощникът за управлявани папки** не е обработен на потребителската пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="14fe1-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="14fe1-106">Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия в облака организация веднъж на всеки седем дни.</span><span class="sxs-lookup"><span data-stu-id="14fe1-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="14fe1-107">Ако промените етикет за съхранение или приложите различни правила за съхранение към пощенска кутия, можете да изчакате докато управлява папка подпомагат обработва пощенската кутия, или можете да стартирате Start-ManagedFolderAssistant cmdlet да започне помощникът за управлявани папки да обработи конкретен пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="14fe1-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="14fe1-108">Работещи тази кратка команда е полезна за тестване или отстраняване на политика на задържане или задържане етикет настройки.</span><span class="sxs-lookup"><span data-stu-id="14fe1-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="14fe1-109">За повече информация посетете [тичам помощникът за управлявани папки](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="14fe1-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="14fe1-110">**Разтвор:** Изпълнете следната команда да започне помощникът за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="14fe1-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="14fe1-111">Това може да възникне и ако **RetentionHold** е било **разрешено** на пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="14fe1-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="14fe1-112">Ако пощенската кутия е бил поставен на RetentionHold, правилото за съхранение за пощенската кутия няма да бъдат обработвани по това време.</span><span class="sxs-lookup"><span data-stu-id="14fe1-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="14fe1-113">За повече информация относно настройката вижте RetentionHold: [Пощенска кутия задържане](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="14fe1-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="14fe1-114">**Решение:**</span><span class="sxs-lookup"><span data-stu-id="14fe1-114">**Solution:**</span></span>
    
  - <span data-ttu-id="14fe1-115">Проверка на състоянието на настройката на RetentionHold на конкретна пощенска кутия в [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="14fe1-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="14fe1-116">Изпълнете следната команда да **забраните** RetentionHold определена пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="14fe1-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="14fe1-117">Сега изпълнете отново папката управлявани помощник:</span><span class="sxs-lookup"><span data-stu-id="14fe1-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="14fe1-118">**Забележка:** Ако пощенската кутия е по-малък от 10 MB, помощникът за управлявани папки ще не автоматично обработва пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="14fe1-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  