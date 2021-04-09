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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645120"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Възстановяване на изтрита група на Microsoft 365

Можете да възстановите изтрита група на Microsoft 365 или Microsoft Teams в рамките на 30 дни от изтриването.

1. Отидете в центъра [за администриране на Microsoft 365,](https://aka.ms/RestoreDeletedGroup) за да влезете в списък с изтрити групи и екипи.

    **Забележка:** Влезте с помощта на акаунта, който е присвоен на администратора на клиента или ролята на администратор на групите.

1. Изберете изтритата група на Microsoft 365/Teams, която да бъде възстановена, и щракнете върху **групата за възстановяване.**

    Ако групата не може да бъде възстановена поради конфликтен SMTP адрес, използвайте следната команда, за да намерите обекта, който причинява конфликт, и премахнете SMTP адреса:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Забележка:** В някои случаи може да отнеме до 24 часа, докато групата и всичките й данни бъдат възстановени.

    За повече информация или за да научите как да възстановявате групи с помощта на PowerShell, вижте [Възстановяване на изтрита група на Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).