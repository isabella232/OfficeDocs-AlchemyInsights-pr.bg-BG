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
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747192"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="75e9d-102">Премести имейл в архивната пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="75e9d-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="75e9d-103">Потвърдете, че **Архив пощенска кутия** е разрешен.</span><span class="sxs-lookup"><span data-stu-id="75e9d-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="75e9d-104">Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) за да активирате архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="75e9d-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="75e9d-105">За да архивирате съобщения автоматично в архивната пощенска кутия, етикет за съхранение с действието за **Преместване в Архив** трябва да се настрои да **прилага автоматично за целия пощенска кутия (по подразбиране) етикет**.</span><span class="sxs-lookup"><span data-stu-id="75e9d-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="75e9d-106">Използвайте стъпки тук, за да създадете етикет: [Архив по подразбиране етикет](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="75e9d-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="75e9d-107">След това добавете **Архив** етикет към вашите правила за задържане.</span><span class="sxs-lookup"><span data-stu-id="75e9d-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="75e9d-108">В центъра за администриране на Exchange изберете **Правила за задържане** > добави **Премести в Архив етикет** към политиката > **записване**.</span><span class="sxs-lookup"><span data-stu-id="75e9d-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="75e9d-109">Сега [присвоите правило за](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) конкретна потребителска пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="75e9d-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="75e9d-110">Същата политика ще бъдат приложени към **основната** , така и за **архивната** пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="75e9d-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="75e9d-111">Тя може да се наложи да принуди управлявана папка помощник (МВНР) да изпълнява и прилага новите настройки за пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="75e9d-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="75e9d-112">Изпълнете следната команда докато [свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да започне помощникът за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="75e9d-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="75e9d-113">За повече информация относно настройването на политика на Архив вижте [Създаване на архив и заличаване правила за пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="75e9d-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

