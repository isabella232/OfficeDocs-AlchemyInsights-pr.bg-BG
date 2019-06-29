---
title: Ограничаване на SharePoint Online до класически режим
ms.author: kirks
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369762"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8d7dd-102">Ограничаване на SharePoint Online до класически режим</span><span class="sxs-lookup"><span data-stu-id="8d7dd-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8d7dd-103">Някои организации все още изискват класически режим опит.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8d7dd-104">Макар че има планове да премахнете класически режим на гранулиран ниво, вече е възможно да се ограничи цялата организация (наемателя) на класически режим за списъци и библиотеки.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8d7dd-105">Администратор ще има следните опции за управление на индивидуални списъци и библиотеки в класически режим, използване на гранулиран неучастие ключове, които предлагаме на следните равнища:</span><span class="sxs-lookup"><span data-stu-id="8d7dd-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8d7dd-106">колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="8d7dd-106">site collection</span></span>
- <span data-ttu-id="8d7dd-107">сайт</span><span class="sxs-lookup"><span data-stu-id="8d7dd-107">site</span></span>
- <span data-ttu-id="8d7dd-108">списък</span><span class="sxs-lookup"><span data-stu-id="8d7dd-108">list</span></span>
- <span data-ttu-id="8d7dd-109">Библиотека</span><span class="sxs-lookup"><span data-stu-id="8d7dd-109">library</span></span>

<span data-ttu-id="8d7dd-110">Освен това списъци, които използват определени функции и персонализации, които не се поддържат от съвременни ще все още се автоматично шибалка към класически режим.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8d7dd-111">Започва на 1 април 2019 г процес, за да забраните на клиентско ниво откажете модерни списъка и библиотеки ще започне и ще продължи до 31 май 2019.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8d7dd-112">Списъците и библиотеките, които са в класически режим в резултат на наемател неучастие автоматично ще се изместят към модерни.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8d7dd-113">Ако имате нужда от класически режим Моля, Вижте повече информация [тук](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) и PnP Powershell Инструкция [тук](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) който описва опции и инструменти, можете да използвате днес за използване на класически режим опит.</span><span class="sxs-lookup"><span data-stu-id="8d7dd-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
