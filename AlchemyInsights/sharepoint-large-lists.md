---
title: Големи списъци на SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767274"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="669a3-102">Работа с големи списъци и библиотеки в SharePoint</span><span class="sxs-lookup"><span data-stu-id="669a3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="669a3-103">Списъците и библиотеките на SharePoint могат да съдържат до 30 милиона елемента, но когато имат повече от 5000 елемента, може да видите грешка в изгледа на списъка при опит за работа с тях.</span><span class="sxs-lookup"><span data-stu-id="669a3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="669a3-104">Този праг е въведен, за да се поддържа производителността на услугата.</span><span class="sxs-lookup"><span data-stu-id="669a3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="669a3-105">Той не може да бъде променян.</span><span class="sxs-lookup"><span data-stu-id="669a3-105">It can't be changed.</span></span> <span data-ttu-id="669a3-106">За да избегнете удрянето на този праг:</span><span class="sxs-lookup"><span data-stu-id="669a3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="669a3-107">**Използвайте модерни**</span><span class="sxs-lookup"><span data-stu-id="669a3-107">**Use modern**</span></span>

<span data-ttu-id="669a3-108">Изгледи, показващи много елементи, работят най-добре в съвременния опит.</span><span class="sxs-lookup"><span data-stu-id="669a3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="669a3-109">[Използвайте съвременния опит,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) за да избегнете грешки, които може да видите в класическия опит.</span><span class="sxs-lookup"><span data-stu-id="669a3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="669a3-110">**Добавяне на индекси**</span><span class="sxs-lookup"><span data-stu-id="669a3-110">**Add indexes**</span></span>

<span data-ttu-id="669a3-111">Когато филтрирате или сортирате по колона, която няма индекс, може да видите съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="669a3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="669a3-112">[Добавете индекс](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ръчно от **Настройки** на списъка в менюто с настройки, след което **индексирани колони**.</span><span class="sxs-lookup"><span data-stu-id="669a3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="669a3-113">**Редактиране на списъчен изглед**</span><span class="sxs-lookup"><span data-stu-id="669a3-113">**Edit the list view**</span></span>

<span data-ttu-id="669a3-114">Ако се появи грешка при работа с голям списък, [редактирайте изгледа на вашия списък](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="669a3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="669a3-115">Следващите четири промени ще премахнат грешките в прага на списъка.</span><span class="sxs-lookup"><span data-stu-id="669a3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="669a3-116">Направете всички четири промени, за да премахнете всички грешки.</span><span class="sxs-lookup"><span data-stu-id="669a3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="669a3-117">Ако все още получавате грешки, проверете [Управление на големи списъци и библиотеки](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="669a3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="669a3-118">Изберете **Няма** от **двете Първо сортиране по колоната** и след това **сортирайте по колоната**.</span><span class="sxs-lookup"><span data-stu-id="669a3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="669a3-119">Изберете **Няма** от **двете Първата група по колоната** и След това група по **колона**.</span><span class="sxs-lookup"><span data-stu-id="669a3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="669a3-120">Изберете **Няма** за всички колони в секцията **Общи суми.**</span><span class="sxs-lookup"><span data-stu-id="669a3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="669a3-121">Премахнете отметката от всички, освен една колона за показване от **раздела Колони.**</span><span class="sxs-lookup"><span data-stu-id="669a3-121">Deselect all but one column for display from the **Columns** section.</span></span>

