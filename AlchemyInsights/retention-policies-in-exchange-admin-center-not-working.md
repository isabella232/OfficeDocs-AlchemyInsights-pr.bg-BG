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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="59cdb-102">Правила за съхранение в центъра за администриране на Exchange</span><span class="sxs-lookup"><span data-stu-id="59cdb-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="59cdb-103">Ако искате да изпълняваме автоматизирани проверки за настройките, упоменати по-долу, изберете бутона Назад < – в горния край на тази страница и след това въведете имейл адреса на потребителя, който има проблеми с правилата за съхранение.</span><span class="sxs-lookup"><span data-stu-id="59cdb-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="59cdb-104">**Проблем:** Новосъздадените или актуализираните правила за съхранение в центъра за администриране на Exchange не се прилагат към пощенските кутии или елементите не се преместват в пощенската кутия или изтриват.</span><span class="sxs-lookup"><span data-stu-id="59cdb-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="59cdb-105">**Главни причини:**</span><span class="sxs-lookup"><span data-stu-id="59cdb-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="59cdb-106">Това може да се дължи на факта, че **Помощникът за управление на папки** не е обработил пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="59cdb-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="59cdb-107">Помощникът за управление на папки се опитва да обработи всяка пощенска кутия във вашата организация, базирана на облак, на всеки седем дни.</span><span class="sxs-lookup"><span data-stu-id="59cdb-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="59cdb-108">Ако промените етикет за съхранение или прилагате други правила за съхранение към пощенска кутия, можете да изчакате, докато управляваната папка помогне за процеса на пощенската кутия, или можете да изпълните кратката команда Start-ManagedFolderAssistant, за да стартирате помощника за управление на папки, за да обработите конкретна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="59cdb-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="59cdb-109">Изпълнението на тази кратка команда е полезно за тестване или отстраняване на неизправности при правила за съхранение или настройки на етикети за съхранение.</span><span class="sxs-lookup"><span data-stu-id="59cdb-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="59cdb-110">За повече информация посетете [изпълнение на помощника за управление на папки](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="59cdb-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="59cdb-111">**Решение:** Изпълнете следната команда, за да стартирате помощника за управление на папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="59cdb-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="59cdb-112">Това може да се случи и ако **RetentionHold** е **разрешена** за пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="59cdb-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="59cdb-113">Ако пощенската кутия е поставена върху RetentionHold, правилата за съхранение в пощенската кутия няма да бъдат обработени през това време.</span><span class="sxs-lookup"><span data-stu-id="59cdb-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="59cdb-114">За повече инсталациите в настройката за RetentionHold вижте: [задържане на съхранение на пощенска кутия](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="59cdb-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="59cdb-115">**Решение**</span><span class="sxs-lookup"><span data-stu-id="59cdb-115">**Solution:**</span></span>
    
  - <span data-ttu-id="59cdb-116">Проверете състоянието на настройката RetentionHold на конкретната пощенска кутия в [ЕКСО PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="59cdb-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="59cdb-117">Изпълнете следната команда, за да **забраните** RetentionHold в конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="59cdb-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="59cdb-118">Сега стартирайте повторно помощника за управление на папки:</span><span class="sxs-lookup"><span data-stu-id="59cdb-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="59cdb-119">**Забележка:** Ако една пощенска кутия е по-малка от 10 МБ, помощникът за управление на папки няма да обработва автоматично пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="59cdb-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="59cdb-120">За повече информация относно правилата за съхранение в центъра за администриране на Exchange вижте:</span><span class="sxs-lookup"><span data-stu-id="59cdb-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="59cdb-121">Етикети за съхранение и правила за съхранение</span><span class="sxs-lookup"><span data-stu-id="59cdb-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="59cdb-122">Прилагане на правила за съхранение към пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="59cdb-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="59cdb-123">Добавяне или премахване на етикети за съхранение</span><span class="sxs-lookup"><span data-stu-id="59cdb-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="59cdb-124">Как да идентифицирате типа на задържане, поставен върху пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="59cdb-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
