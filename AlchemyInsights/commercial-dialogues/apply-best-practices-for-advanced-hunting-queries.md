---
title: Прилагане на най-добри практики за разширени ловни заявки
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743705"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="ac3ef-102">Прилагане на най-добри практики за разширени ловни заявки</span><span class="sxs-lookup"><span data-stu-id="ac3ef-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="ac3ef-103">За да получите резултати по-бързо и за да избегнете таймаут при изпълнение на сложни заявки, приложете тези най-добри практики:</span><span class="sxs-lookup"><span data-stu-id="ac3ef-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="ac3ef-104">Когато се опитвате нови заявки, винаги използвайте ограничението, за да избегнете получаването на изключително големи набори от резултати.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="ac3ef-105">Можете също да използвате, `count` за да направите първоначална оценка на размера на набора от резултати.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="ac3ef-106">Използвайте първо филтри за време.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-106">Use time filters first.</span></span> <span data-ttu-id="ac3ef-107">В идеалния случай, Ограничете заявките до седем дни.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="ac3ef-108">В началото на заявка веднага след филтъра за време Добавете филтрите, които се очаква да премахнат повечето от данните.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="ac3ef-109">Когато търсите пълни маркери, използвайте `has` оператора вместо това `contains` .</span><span class="sxs-lookup"><span data-stu-id="ac3ef-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="ac3ef-110">Извършете търсене в определена колона вместо във всички колони.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="ac3ef-111">Когато се присъединявате към таблици, първо Задайте таблицата с по-малко редове.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="ac3ef-112">`project` само необходимите колони от таблиците, към които сте се присъединили.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="ac3ef-113">За да научите повече, вижте [най-добри практики при заявка](https://go.microsoft.com/fwlink/?linkid=2144812)за търсене.</span><span class="sxs-lookup"><span data-stu-id="ac3ef-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
