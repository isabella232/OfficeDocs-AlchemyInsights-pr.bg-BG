---
title: Пощенската ви кутия за архивиране е почти пълна
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974179"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="78c00-102">Пощенската ви кутия за архивиране е почти пълна</span><span class="sxs-lookup"><span data-stu-id="78c00-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="78c00-103">Ако потребителят получи предупреждение; **Пощенската ви кутия за архивиране е почти пълна** или трябва да увеличите размера на тяхната архивна пощенска кутия, Ето някои съвети:</span><span class="sxs-lookup"><span data-stu-id="78c00-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="78c00-104">Ако на потребителя е присвоен абонамент за Exchange Online (план 1), преминете към лиценза за **Exchange Online (план 2** ), за да увеличите размера от 50 ГБ към 100 GB.</span><span class="sxs-lookup"><span data-stu-id="78c00-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="78c00-105">Ако потребителят вече е възложил някое от следните неща: **план 2 за Exchange Online** или Exchange Online (план 1) с добавка за архивиране на Exchange Online, използвайте стъпките по-долу, за да разрешите автоматичното разширяване на архивирането:.</span><span class="sxs-lookup"><span data-stu-id="78c00-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="78c00-106">[Свързване към PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="78c00-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="78c00-107">Изпълнете следните команда Set unifiedgroup за потребителя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="78c00-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="78c00-108">Изпълнете следните команда Set unifiedgroup, за да потвърдите, че е разрешена за потребителя:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="78c00-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="78c00-109">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="78c00-109">For more information see:</span></span>

- [<span data-ttu-id="78c00-110"> Разрешаване на неограничени архивиране – помощ за администратори – Microsoft 365 съответствие | Документи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="78c00-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="78c00-111">Ограничения за Exchange Online – описания на услугите | Документи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="78c00-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="78c00-112">Надстройване до различен бизнес план | Документи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="78c00-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

