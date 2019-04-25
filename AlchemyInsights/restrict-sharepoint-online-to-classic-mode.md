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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422164"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c3a8a-102">Ограничаване на SharePoint Online до класически режим</span><span class="sxs-lookup"><span data-stu-id="c3a8a-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c3a8a-103">Някои организации все още изискват класически режим опит.</span><span class="sxs-lookup"><span data-stu-id="c3a8a-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c3a8a-104">Макар че има планове да премахнете класически режим на гранулиран ниво, започваща април 1,2019, то вече няма да е възможно да се ограничи цялата организация (наемателя) в класически режим за списъци и библиотеки.</span><span class="sxs-lookup"><span data-stu-id="c3a8a-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c3a8a-105">Администратор ще има следните опции за управление на индивидуални списъци и библиотеки в класически режим, използване на гранулиран неучастие ключове, които предлагаме на следните равнища:</span><span class="sxs-lookup"><span data-stu-id="c3a8a-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c3a8a-106">колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="c3a8a-106">site collection</span></span>
- <span data-ttu-id="c3a8a-107">сайт</span><span class="sxs-lookup"><span data-stu-id="c3a8a-107">site</span></span>
- <span data-ttu-id="c3a8a-108">списък</span><span class="sxs-lookup"><span data-stu-id="c3a8a-108">list</span></span>
- <span data-ttu-id="c3a8a-109">Библиотека</span><span class="sxs-lookup"><span data-stu-id="c3a8a-109">library</span></span>

<span data-ttu-id="c3a8a-110">Освен това списъци, които използват определени функции и персонализации, които не се поддържат от съвременни ще все още се автоматично шибалка към класически режим.</span><span class="sxs-lookup"><span data-stu-id="c3a8a-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c3a8a-111">След 1 април списъци и библиотеки, които са в класически режим в резултат на наемател неучастие автоматично ще се управляват на ниво сайт и ниво на списъка.</span><span class="sxs-lookup"><span data-stu-id="c3a8a-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="c3a8a-112">Ако имате нужда от класически режим Моля, Вижте повече информация тук и PnP Powershell Инструкция тук, която описва опции и инструменти, можете да използвате днес да се подготвят за отстраняването на клиентско ниво неучастие на 1 април.</span><span class="sxs-lookup"><span data-stu-id="c3a8a-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
