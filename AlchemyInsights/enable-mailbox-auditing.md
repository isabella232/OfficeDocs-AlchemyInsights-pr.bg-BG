---
title: Разрешаване на проверка на пощенските кутии
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806280"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="28178-102">Разрешаване на проверка на пощенските кутии</span><span class="sxs-lookup"><span data-stu-id="28178-102">Enable mailbox auditing</span></span>

<span data-ttu-id="28178-103">За да разрешите проверка на пощенските кутии за отделен потребител или за цялата организация, трябва да изпълните следните кратки команди от отдалечен Power Shell:</span><span class="sxs-lookup"><span data-stu-id="28178-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="28178-104">**Отделен потребител**</span><span class="sxs-lookup"><span data-stu-id="28178-104">**Single User**</span></span>
  
<span data-ttu-id="28178-105">Set-пощенска кутия-самоличност "Джейн Дау"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="28178-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="28178-106">**Организация**</span><span class="sxs-lookup"><span data-stu-id="28178-106">**Organization**</span></span>
  
<span data-ttu-id="28178-107">Получаване на пощенска кутия – ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-пощенска кутия – AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="28178-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="28178-108">Научете повече</span><span class="sxs-lookup"><span data-stu-id="28178-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

