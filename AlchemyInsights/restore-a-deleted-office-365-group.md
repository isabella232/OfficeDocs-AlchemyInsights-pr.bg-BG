---
title: Възстановяване на изтрита Microsoft 365 група
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959015"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Възстановяване на изтрита Microsoft 365 група

Можете да възстановите изтрита Microsoft 365 или да Microsoft Teams в рамките на 30 дни от изтриването.

1. Отидете на [Център за администриране на Microsoft 365,](https://aka.ms/RestoreDeletedGroup) за да влезете в списък на изтритите групи и екипи.

    **Забележка:** Влезте с помощта на акаунта, който е присвоен на администратора на клиента или ролята на администратор на групите.

1. Изберете изтритата Microsoft 365/Teams, която да бъде възстановена, и щракнете върху **групата за възстановяване.**

    Ако групата не може да бъде възстановена поради конфликтен SMTP адрес, използвайте следната команда, за да намерите обекта, който причинява конфликт, и премахнете SMTP адреса:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Забележка:** В някои случаи може да отнеме до 24 часа, докато групата и всичките й данни бъдат възстановени.

    За повече информация или за да научите как да възстановите групи с помощта на PowerShell, вижте [Възстановяване на изтрита Microsoft 365 група](https://go.microsoft.com/fwlink/?linkid=867802).