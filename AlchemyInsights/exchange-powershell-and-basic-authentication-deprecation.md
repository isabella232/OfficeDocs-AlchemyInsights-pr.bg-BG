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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="bac00-102">Exchange PowerShell и отхвърляне на базово удостоверяване</span><span class="sxs-lookup"><span data-stu-id="bac00-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="bac00-103">За най-новата информация за това как да се свържете към PowerShell в Exchange Online без използване на базово удостоверяване, [отидете тук](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="bac00-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="bac00-104">Обърнете внимание, че базовото удостоверяване все още трябва да бъде разрешено на вашия клиентски компютър.</span><span class="sxs-lookup"><span data-stu-id="bac00-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="bac00-105">Новият модул за PowerShell V2 използва модерното удостоверяване, за да установи връзка за разрешаването на всички базирани на REST команди на V2.</span><span class="sxs-lookup"><span data-stu-id="bac00-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="bac00-106">В допълнение към кратките команди на V2, той също така ви позволява да имате достъп до по-старите команди за Remote PowerShell (RPS), които изискват установяване на отдалечена сесия на PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bac00-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="bac00-107">Създаването на сесия на RPS на компютър с Windows изисква базовото удостоверяване на WinRM да бъде разрешено на клиентския компютър, въпреки че модулът използва модерен механизъм за удостоверяване на услугата.</span><span class="sxs-lookup"><span data-stu-id="bac00-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="bac00-108">Каналът за базово удостоверяване на WinRM се използва за пренос на модерни маркери за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="bac00-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="bac00-109">Ако базовото удостоверяване на WinRM е дезактивирано на клиентския компютър, новите команди на V2 ще продължат да работят (но по-старите кратки команди на RPS няма да работят с него).</span><span class="sxs-lookup"><span data-stu-id="bac00-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
