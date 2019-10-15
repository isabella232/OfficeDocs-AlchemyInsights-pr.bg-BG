---
title: Големи списъци на SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488506"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="6dc29-102">Работа с големи списъци и библиотеки в SharePoint</span><span class="sxs-lookup"><span data-stu-id="6dc29-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="6dc29-103">Списъците и библиотеките на SharePoint могат да съдържат до 30 000 000 елемента, но когато имат повече от 5 000 елемента, може да видите грешка в Прага на списъчен изглед, когато се опитвате да работите с тях.</span><span class="sxs-lookup"><span data-stu-id="6dc29-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="6dc29-104">Този праг е налице, за да се поддържа изпълнението на услугата.</span><span class="sxs-lookup"><span data-stu-id="6dc29-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="6dc29-105">Не може да се промени.</span><span class="sxs-lookup"><span data-stu-id="6dc29-105">It can't be changed.</span></span> <span data-ttu-id="6dc29-106">За да избегнете натискане на този праг:</span><span class="sxs-lookup"><span data-stu-id="6dc29-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="6dc29-107">**Използвайте модерни**</span><span class="sxs-lookup"><span data-stu-id="6dc29-107">**Use modern**</span></span>

<span data-ttu-id="6dc29-108">Изгледите, показващи много елементи, работят най-добре в съвременния опит.</span><span class="sxs-lookup"><span data-stu-id="6dc29-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="6dc29-109">[Използвайте съвременния опит](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , за да избегнете грешки, които може да видите в класическото преживяване.</span><span class="sxs-lookup"><span data-stu-id="6dc29-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="6dc29-110">**Добавяне на индекси**</span><span class="sxs-lookup"><span data-stu-id="6dc29-110">**Add indexes**</span></span>

<span data-ttu-id="6dc29-111">Когато филтрирате или сортирате по колона, която няма индекс, може да видите съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="6dc29-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="6dc29-112">[Добавете индекс](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ръчно от **настройките на списъка** в менюто с настройки, след което **индексирани колони**.</span><span class="sxs-lookup"><span data-stu-id="6dc29-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="6dc29-113">**Редактиране на списъчен изглед**</span><span class="sxs-lookup"><span data-stu-id="6dc29-113">**Edit the list view**</span></span>

<span data-ttu-id="6dc29-114">Ако възникне грешка при работа с голям списък, [редактирайте изгледа на списъка](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="6dc29-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="6dc29-115">Следните четири промени ще премахнат грешките в списъчното виждане.</span><span class="sxs-lookup"><span data-stu-id="6dc29-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="6dc29-116">Направете всички четири промени, за да премахнете всички грешки.</span><span class="sxs-lookup"><span data-stu-id="6dc29-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="6dc29-117">Ако все още получавате грешки, проверете [управлението на големи списъци и библиотеки](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="6dc29-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="6dc29-118">Изберете **не** от **първо сортиране по колоната** и **след това сортиране по колоната**.</span><span class="sxs-lookup"><span data-stu-id="6dc29-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="6dc29-119">Изберете **няма** от **първата група от колоната** и **след това групирайте по колоната**.</span><span class="sxs-lookup"><span data-stu-id="6dc29-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="6dc29-120">Изберете **няма** за всички колони в раздела **Общи** .</span><span class="sxs-lookup"><span data-stu-id="6dc29-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="6dc29-121">Премахнете отметката от всички, освен от една колона за показване от секцията **колони** .</span><span class="sxs-lookup"><span data-stu-id="6dc29-121">Deselect all but one column for display from the **Columns** section.</span></span>

