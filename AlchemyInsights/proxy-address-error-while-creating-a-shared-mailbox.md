---
title: Грешка за адрес на прокси сървър при създаването на споделена пощенска кутия
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568279"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="5083d-102">Грешка за адрес на прокси сървър при създаването на пощенска кутия или друг обект с активиран имейл</span><span class="sxs-lookup"><span data-stu-id="5083d-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="5083d-103">Ако сте се опитали да създадете обект с активиран имейл (пощенска кутия, споделена пощенска кутия и т. н.) и сте получили грешката "прокси адресът" SMTP:alias@domain.com "вече се използва...", имейл адресът, който сте избрали, вече е зает от друг обект с активиран имейл във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="5083d-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="5083d-104">Трябва да намерите потребителя, групата, споделената пощенска кутия или публичната папка с този имейл адрес и да я изтриете или да промените неговия имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="5083d-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="5083d-105">След това можете да създадете нов обект с активиран имейл</span><span class="sxs-lookup"><span data-stu-id="5083d-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="5083d-106">Използвайте търсене на началната страница, за да го намерите.</span><span class="sxs-lookup"><span data-stu-id="5083d-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="5083d-107">Можете също да използвате командата по-долу в Exchange Online PowerShell, за да я потърсите:</span><span class="sxs-lookup"><span data-stu-id="5083d-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="5083d-108">Ако не искате да изтривате съществуващия имейл адрес, изберете нов имейл адрес за новия обект, който създавате.</span><span class="sxs-lookup"><span data-stu-id="5083d-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  