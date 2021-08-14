---
title: Грешка в адреса на прокси сървъра при създаване на споделена пощенска кутия
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062897"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Грешка в адреса на прокси сървъра при създаване на пощенска кутия или друг обект с разрешен имейл

Ако сте се опитали да създадете обект с активиран имейл (пощенска кутия, споделена пощенска кутия и т.н.) и сте получили грешката "Адресът на прокси сървъра "SMTP:alias@domain.com" вече се използва...", имейл адресът, който сте избрали, вече е взет от друг обект с активиран имейл във вашата организация.
  
Трябва да намерите потребителя, групата, споделената пощенска кутия или публичната папка, която има този имейл адрес, и да го изтриете или да промените имейл адреса му. След това можете да създадете нов обект с активиран имейл с безплатния имейл адрес. Използвайте "Търсене" на началната страница, за да го намерите. Можете също да използвате следната команда Exchange Online PowerShell, за да я търсите:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ако не искате да изтриете съществуващия имейл адрес, изберете нов имейл адрес за новия обект, който създавате.
  