---
title: Местоположение на данните
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655271"
---
# <a name="data-location"></a><span data-ttu-id="e2c81-102">Местоположение на данните</span><span class="sxs-lookup"><span data-stu-id="e2c81-102">Data location</span></span>

<span data-ttu-id="e2c81-103">Можете да видите местоположението на вашия клиент в центъра за администриране или чрез свързване към Exchange Online чрез PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e2c81-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="e2c81-104">**Център за администриране:**</span><span class="sxs-lookup"><span data-stu-id="e2c81-104">**Admin center:**</span></span>
1. <span data-ttu-id="e2c81-105">Влезте в [центъра за администриране](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="e2c81-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="e2c81-106">Изберете **Настройки на** > **организацията профил**.</span><span class="sxs-lookup"><span data-stu-id="e2c81-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="e2c81-107">Под **Местоположение на данните**изберете Преглед на подробни **данни**.</span><span class="sxs-lookup"><span data-stu-id="e2c81-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="e2c81-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="e2c81-108">**PowerShell:**</span></span>
1. <span data-ttu-id="e2c81-109">Свързване с Exchange Online чрез Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e2c81-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="e2c81-110">Изпълнение на кратката команда [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) да покаже списък на свойствата на вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="e2c81-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="e2c81-111">Погледнете свойството OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="e2c81-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="e2c81-112">Когато имате местоположението на данните за EXO и SPO, можете да определите местоположението на данните за други услуги, които можете да използвате от [Мястото, където се намират данните ви](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="e2c81-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>