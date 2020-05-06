---
title: Exchange PowerShell и отхвърляне на базово удостоверяване
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015678"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell и отхвърляне на базово удостоверяване

За най-новата информация за това как да се свържете към PowerShell в Exchange Online без използване на базово удостоверяване, [отидете тук](https://aka.ms/psbasicauth).

Обърнете внимание, че базовото удостоверяване все още трябва да бъде разрешено на вашия клиентски компютър.
Новият модул за PowerShell V2 използва модерното удостоверяване, за да установи връзка за разрешаването на всички базирани на REST команди на V2. В допълнение към кратките команди на V2, той също така ви позволява да имате достъп до по-старите команди за Remote PowerShell (RPS), които изискват установяване на отдалечена сесия на PowerShell. Създаването на сесия на RPS на компютър с Windows изисква базовото удостоверяване на WinRM да бъде разрешено на клиентския компютър, въпреки че модулът използва модерен механизъм за удостоверяване на услугата. Каналът за базово удостоверяване на WinRM се използва за пренос на модерни маркери за удостоверяване. Ако базовото удостоверяване на WinRM е дезактивирано на клиентския компютър, новите команди на V2 ще продължат да работят (но по-старите кратки команди на RPS няма да работят с него).
