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
# <a name="your-archive-mailbox-is-almost-full"></a>Пощенската ви кутия за архивиране е почти пълна

Ако потребителят получи предупреждение; **Пощенската ви кутия за архивиране е почти пълна** или трябва да увеличите размера на тяхната архивна пощенска кутия, Ето някои съвети:

1. Ако на потребителя е присвоен абонамент за Exchange Online (план 1), преминете към лиценза за **Exchange Online (план 2** ), за да увеличите размера от 50 ГБ към 100 GB.
1. Ако потребителят вече е възложил някое от следните неща: **план 2 за Exchange Online** или Exchange Online (план 1) с добавка за архивиране на Exchange Online, използвайте стъпките по-долу, за да разрешите автоматичното разширяване на архивирането:.
 
    1. [Свързване към PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Изпълнете следните команда Set unifiedgroup за потребителя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Изпълнете следните команда Set unifiedgroup, за да потвърдите, че е разрешена за потребителя:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

За повече информация вижте:

- [ Разрешаване на неограничени архивиране – помощ за администратори – Microsoft 365 съответствие | Документи на Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Ограничения за Exchange Online – описания на услугите | Документи на Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Надстройване до различен бизнес план | Документи на Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

