---
title: Ограничаване на SharePoint Online в класически режим
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752057"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="cc539-102">Ограничаване на SharePoint Online в класически режим</span><span class="sxs-lookup"><span data-stu-id="cc539-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="cc539-103">Някои организации все още изискват класически режим опит.</span><span class="sxs-lookup"><span data-stu-id="cc539-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="cc539-104">Въпреки че няма планове за премахване на класическия режим на ниво грануларен, вече не е възможно да ограничите цялата организация (наемател) в класическия режим за списъци и библиотеки.</span><span class="sxs-lookup"><span data-stu-id="cc539-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="cc539-105">Администраторът ще има следните опции за управление на отделни списъци и библиотеки в класически режим, като се използват гранулирани превключватели за отказване, които предоставяме на следните нива:</span><span class="sxs-lookup"><span data-stu-id="cc539-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="cc539-106">колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="cc539-106">site collection</span></span>
- <span data-ttu-id="cc539-107">Сайт</span><span class="sxs-lookup"><span data-stu-id="cc539-107">site</span></span>
- <span data-ttu-id="cc539-108">Списък</span><span class="sxs-lookup"><span data-stu-id="cc539-108">list</span></span>
- <span data-ttu-id="cc539-109">Библиотека</span><span class="sxs-lookup"><span data-stu-id="cc539-109">library</span></span>

<span data-ttu-id="cc539-110">Освен това списъците, които използват определени функции и персонализации, които не се поддържат от съвременните, все още ще бъдат автоматично включени в класическия режим.</span><span class="sxs-lookup"><span data-stu-id="cc539-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="cc539-111">Започвайки 1 април 2019, процесът за забраняване на ниво клиент отказване от модерен списък и библиотеки ще започне и да продължи през май 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="cc539-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="cc539-112">Списъците и библиотеките, които са в класически режим в резултат на отписване на наемател, автоматично ще бъдат преместени в модерен.</span><span class="sxs-lookup"><span data-stu-id="cc539-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="cc539-113">Ако имате нужда от класически режим, моля, Вижте повече информация [тук](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) и програми за ПНП PowerShell [тук](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , които описват опциите и инструментите, които можете да използвате днес, за да използвате класическия режим на работа.</span><span class="sxs-lookup"><span data-stu-id="cc539-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
