---
title: Ограничаване на SharePoint Online до класически режим
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742458"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a6a52-102">Ограничаване на SharePoint Online до класически режим</span><span class="sxs-lookup"><span data-stu-id="a6a52-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a6a52-103">Някои организации все още изискват класически режим опит.</span><span class="sxs-lookup"><span data-stu-id="a6a52-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a6a52-104">Въпреки че няма планове за премахване на класически режим на ниво гранули, вече не е възможно да се ограничи цялата организация (клиент) до класически режим за списъци и библиотеки.</span><span class="sxs-lookup"><span data-stu-id="a6a52-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a6a52-105">Администраторът ще има следните опции за управление на отделни списъци и библиотеки в класически режим с помощта на подробни превключватели за отказване, които предоставяме на следните нива:</span><span class="sxs-lookup"><span data-stu-id="a6a52-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="a6a52-106">колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="a6a52-106">site collection</span></span>
- <span data-ttu-id="a6a52-107">Сайт</span><span class="sxs-lookup"><span data-stu-id="a6a52-107">site</span></span>
- <span data-ttu-id="a6a52-108">Списък</span><span class="sxs-lookup"><span data-stu-id="a6a52-108">list</span></span>
- <span data-ttu-id="a6a52-109">Библиотека</span><span class="sxs-lookup"><span data-stu-id="a6a52-109">library</span></span>

<span data-ttu-id="a6a52-110">Освен това списъците, които използват определени функции и персонализации, които не се поддържат от модерния, ще продължат да се превключват автоматично към класически режим.</span><span class="sxs-lookup"><span data-stu-id="a6a52-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a6a52-111">Началото на 1 април 2019, процесът на деактивиране на ниво клиент отписване от съвременния списък и библиотеки ще започне и да продължи до 31 май 2019.</span><span class="sxs-lookup"><span data-stu-id="a6a52-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="a6a52-112">Списъците и библиотеките, които са в класически режим в резултат на отказ от клиент автоматично ще бъдат прехвърлени към модерни.</span><span class="sxs-lookup"><span data-stu-id="a6a52-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="a6a52-113">Ако се нуждаете от класически режим, моля, вижте повече информация [тук](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) и PnP Powershell инструкция [тук,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) която описва опции и инструменти, които можете да използвате днес, за да използвате класическия режим.</span><span class="sxs-lookup"><span data-stu-id="a6a52-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
