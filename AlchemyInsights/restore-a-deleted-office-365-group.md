---
title: Възстановяване на изтрита група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505671"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Възстановяване на изтрита група на Microsoft 365

Можете да възстановите изтрита група на Microsoft 365 или Microsoft Teams в рамките на 30 дни от изтриването.

1. За да влезете в центъра за администриране на Microsoft 365 и да изброите изтритите групи и екипи, отидете в центъра за администриране на [Microsoft 365](https://aka.ms/RestoreDeletedGroup).

    **Забележка:** Влезте с помощта на акаунта, който е присвоен на администратора на клиента или ролята на администратор на групите.

1. Изберете изтритата група на Microsoft 365/Teams, която да бъде възстановена, и щракнете върху **групата за възстановяване.**

    Ако групата не може да бъде възстановена поради конфликтен SMTP адрес, използвайте следната команда, за да намерите обекта, който причинява конфликт, и премахнете SMTP адреса:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Забележка:** В някои случаи може да отнеме до 24 часа, докато групата и всичките й данни бъдат възстановени.

    За повече информация или за да научите как да възстановявате групи с помощта на PowerShell, вижте [Възстановяване на изтрита група на Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).