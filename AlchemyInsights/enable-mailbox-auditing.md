---
title: Разрешаване на проверка на пощенската кутия
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736242"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="ae21b-102">Разрешаване на проверка на пощенската кутия</span><span class="sxs-lookup"><span data-stu-id="ae21b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="ae21b-103">За да разрешите проверка на пощенската кутия за един потребител или цяла организация следните кратки команди трябва да се изпълняват от отдалечената Power Shell:</span><span class="sxs-lookup"><span data-stu-id="ae21b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="ae21b-104">**Единичен потребител**</span><span class="sxs-lookup"><span data-stu-id="ae21b-104">**Single User**</span></span>
  
<span data-ttu-id="ae21b-105">Set-пощенска кутия-идентичност "Jane Dow"-Аудиоled $true</span><span class="sxs-lookup"><span data-stu-id="ae21b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="ae21b-106">**Организация**</span><span class="sxs-lookup"><span data-stu-id="ae21b-106">**Organization**</span></span>
  
<span data-ttu-id="ae21b-107">Get-пощенска кутия Резултитразмер неограничен-филтър {РеЦипиенттипедетаилс-EQ "UserMailbox кутия"} | Set-пощенска кутия-Аудиоled $true</span><span class="sxs-lookup"><span data-stu-id="ae21b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="ae21b-108">Научете повече</span><span class="sxs-lookup"><span data-stu-id="ae21b-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

