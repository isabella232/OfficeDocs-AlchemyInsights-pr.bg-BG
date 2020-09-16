---
title: MC210173 – SharePoint Designer – прекратяване на функцията за нов формуляр по избор
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743742"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="51a80-102">MC210173 – SharePoint Designer – прекратяване на функцията за нов формуляр по избор</span><span class="sxs-lookup"><span data-stu-id="51a80-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="51a80-103">Установихме проблем, засягащ функционалността на SharePoint Designer за [създаване на персонализирани формуляри](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="51a80-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="51a80-104">След внимателен преглед установихме, че няма известна корекция за този проблем и избрахме да забраним функцията за създаване на персонализиран формуляр, което влиза в сила в 3:00 преди обяд UTC в събота, 25 април 2020 г.</span><span class="sxs-lookup"><span data-stu-id="51a80-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="51a80-105">Тази промяна не оказва влияние върху възможността за редактиране на предварително създадени формуляри, или върху други съществуващи функции в SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="51a80-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="51a80-106">След като е направена тази промяна, възможно е потребителите да са получили грешката: "Не може да се запишат промените в списъка в сървъра" при създаване на нови формуляри.</span><span class="sxs-lookup"><span data-stu-id="51a80-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="51a80-107">Потребителите, които преди това са използвали SharePoint Designer за създаване на персонализирани формуляри, могат вместо това да използват [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) за тази цел.</span><span class="sxs-lookup"><span data-stu-id="51a80-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="51a80-108">PowerApps е лесен и мощен инструмент, който позволява на потребителите да работят в модерната среда на SharePoint Online, за да създават и редактират персонализирани формуляри за списъци в SharePoint и библиотеки с документи директно от прозореца на браузъра.</span><span class="sxs-lookup"><span data-stu-id="51a80-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="51a80-109">PowerApps не изисква традиционните знания за кодиране или някакви допълнителни изтегляния на приложения, например InfoPath.</span><span class="sxs-lookup"><span data-stu-id="51a80-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="51a80-110">**Бележка**: Потребителите на класическата среда в SharePoint Online ще трябва временно да преминат към работа в модерна среда, за да имат достъп и да използват PowerApps; въпреки че до всички персонализирани формуляри, създадени в PowerApps, потребителите на класическата среда в SharePoint Online имат достъп.</span><span class="sxs-lookup"><span data-stu-id="51a80-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
