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
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Грешка за адрес на прокси сървър при създаването на пощенска кутия или друг обект с активиран имейл

Ако сте се опитали да създадете обект с активиран имейл (пощенска кутия, споделена пощенска кутия и т. н.) и сте получили грешката "прокси адресът" SMTP:alias@domain.com "вече се използва...", имейл адресът, който сте избрали, вече е зает от друг обект с активиран имейл във вашата организация.
  
Трябва да намерите потребителя, групата, споделената пощенска кутия или публичната папка с този имейл адрес и да я изтриете или да промените неговия имейл адрес. След това можете да създадете нов обект с активиран имейл Използвайте търсене на началната страница, за да го намерите. Можете също да използвате командата по-долу в Exchange Online PowerShell, за да я потърсите:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ако не искате да изтривате съществуващия имейл адрес, изберете нов имейл адрес за новия обект, който създавате.
  