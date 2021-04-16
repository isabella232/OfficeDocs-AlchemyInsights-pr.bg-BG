---
title: Exchange PowerShell и отхвърляне на базово удостоверяване
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813461"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell и отхвърляне на базово удостоверяване

За най-новата информация за това как да се свържете към PowerShell в Exchange Online без използване на базово удостоверяване, [отидете тук](https://aka.ms/exops-docs). Модулът PowerShell V2 не използва базово удостоверяване.

Обърнете внимание, че базовото удостоверяване все още трябва да бъде разрешено на вашия клиентски компютър.
Новият модул за PowerShell V2 използва модерното удостоверяване, за да установи връзка за разрешаването на всички базирани на REST команди на V2. В допълнение към кратките команди на V2, той също така ви позволява да имате достъп до по-старите команди за Remote PowerShell (RPS), които изискват установяване на отдалечена сесия на PowerShell. Създаването на сесия на RPS на компютър с Windows изисква базовото удостоверяване на WinRM да бъде разрешено на клиентския компютър, въпреки че модулът използва модерен механизъм за удостоверяване на услугата. Каналът за базово удостоверяване на WinRM се използва за пренос на модерни маркери за удостоверяване. Ако базовото удостоверяване на WinRM е дезактивирано на клиентския компютър, новите команди на V2 ще продължат да работят (но по-старите кратки команди на RPS няма да работят с него).
