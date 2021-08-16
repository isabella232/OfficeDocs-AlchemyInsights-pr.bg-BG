---
title: Вашата архивна пощенска кутия е почти пълна
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046741"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Вашата архивна пощенска кутия е почти пълна

Ако потребителят получи предупреждението; **Вашата архивна пощенска кутия е почти пълна** или трябва да увеличите размера на архивната им пощенска кутия, ето някои съвети:

1. Ако на потребителя е даден лиценз за Exchange Online 1, надстройте до Exchange Online на план **2,** за да увеличите размера от 50 ГБ на 100 ГБ.
1. Ако на потребителя вече е възложено едно от следните неща: Exchange Online план **2** или план 1 на Exchange Online с добавка архивиране с Exchange Online, използвайте стъпките по-долу, за да разрешите автоматичното архивиране с разгъване:.
 
    1. [Свързване към Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Изпълнете следната команда за потребителя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Изпълнете следната команда, за да потвърдите, че е разрешена за потребителя:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

За повече информация вижте:

- [Разрешаване на неограничено архивиране – помощ за администратори – Microsoft 365 съответствие | Документи на Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online – описания на услуги | Документи на Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Надстройване до друг бизнес план | Документи на Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

