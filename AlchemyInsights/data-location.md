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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627835"
---
# <a name="data-location"></a><span data-ttu-id="fda5e-102">Местоположение на данните</span><span class="sxs-lookup"><span data-stu-id="fda5e-102">Data location</span></span>

<span data-ttu-id="fda5e-103">Можете да видите местоположението на вашия Office 365 клиент в центъра за администриране или чрез свързване към Exchange Online чрез PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fda5e-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="fda5e-104">**Център за администриране:**</span><span class="sxs-lookup"><span data-stu-id="fda5e-104">**Admin center:**</span></span>
1. <span data-ttu-id="fda5e-105">Влезте в центъра за [администриране](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="fda5e-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="fda5e-106">Изберете **Настройки** > **организационен профил**.</span><span class="sxs-lookup"><span data-stu-id="fda5e-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="fda5e-107">Под **местоположение на данни**изберете **Преглед на подробностите**.</span><span class="sxs-lookup"><span data-stu-id="fda5e-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="fda5e-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="fda5e-108">**PowerShell:**</span></span>
1. <span data-ttu-id="fda5e-109">Свързване с Exchange Online с помощта на Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fda5e-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="fda5e-110">Изпълнение на кратката команда [get-Организацияединица](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) за показване на списък на свойствата на вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="fda5e-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="fda5e-111">Вижте собствеността на Организацияид.</span><span class="sxs-lookup"><span data-stu-id="fda5e-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="fda5e-112">Когато имате местоположението на данните за ЕКЗО и спо, можете да определите местоположението на данните за други услуги, които можете да използвате от [мястото, където се намират вашите данни](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="fda5e-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>