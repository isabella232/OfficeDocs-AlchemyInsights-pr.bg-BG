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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597432"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Възстановяване на изтрита група на Microsoft 365

Можете да възстановите изтрита група на Microsoft 365 или Microsoft Teams в рамките на 30 дни от изтриването.

1. Отидете в центъра [за администриране на Microsoft 365,](https://aka.ms/RestoreDeletedGroup) за да влезете и да изброите изтритите групи и екипи.

    **Забележка:** Влезте с помощта на акаунта, който е присвоен на администратора на клиента или ролята на администратор на групите.

1. Изберете изтритата група на Microsoft 365/Teams, която да бъде възстановена, и щракнете върху **групата за възстановяване.**

    Ако групата не може да бъде възстановена поради конфликтен SMTP адрес, използвайте следната команда, за да намерите обекта, който причинява конфликт, и премахнете SMTP адреса:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Забележка:** В някои случаи може да отнеме до 24 часа, докато групата и всичките й данни бъдат възстановени.

    За повече информация или за да научите как да възстановявате групи с помощта на PowerShell, вижте [Възстановяване на изтрита група на Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).