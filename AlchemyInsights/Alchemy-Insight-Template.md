---
title: същото като името на файла е най-добре
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800034"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="1b18b-102">Задължителна алхимията заглавка H1, H2's не работят.</span><span class="sxs-lookup"><span data-stu-id="1b18b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="1b18b-103">Най-добри практики и насоки за авторство алхимията:</span><span class="sxs-lookup"><span data-stu-id="1b18b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="1b18b-104">**Не Гнездете прозрения алхимията в папките**-това ще прекъсне структурата на URL.</span><span class="sxs-lookup"><span data-stu-id="1b18b-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="1b18b-105">Опитваме се да го поправяме.</span><span class="sxs-lookup"><span data-stu-id="1b18b-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="1b18b-106">Файловете в папката **Alchemyinsights данни** трябва да имат малки имена на файлове с тирета за интервали ex.</span><span class="sxs-lookup"><span data-stu-id="1b18b-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="1b18b-107">" ***как да се разреши***"-задържане.</span><span class="sxs-lookup"><span data-stu-id="1b18b-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="1b18b-108">Включете идентификационния номер на правилото или идентификационния номер на кофата от [портала за партньори алхимията](https://alchemyportal.azurewebsites.net) в полето по избор на MS.</span><span class="sxs-lookup"><span data-stu-id="1b18b-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="1b18b-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="1b18b-109">ex.</span></span> <span data-ttu-id="1b18b-110">***MS. обичай: 100021***</span><span class="sxs-lookup"><span data-stu-id="1b18b-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="1b18b-111">Използвайте останалата част от метаданните в горната част на този файл като шаблон.</span><span class="sxs-lookup"><span data-stu-id="1b18b-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="1b18b-112">В [портала за партньори алхимията](https://alchemyportal.azurewebsites.net)Придвижете се до секцията " **вникване** в раздела" на клиента: и използвайте това като отправна точка за заглавието на вашето име H1 за вникване.</span><span class="sxs-lookup"><span data-stu-id="1b18b-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="1b18b-113">Статистиката на алхимията трябва да има само един H1 в горната част или те ще се счупят в производството.</span><span class="sxs-lookup"><span data-stu-id="1b18b-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="1b18b-114">H2s не правят така, че да използват **смели** или други конвенции за обозначаване на отделни секции.</span><span class="sxs-lookup"><span data-stu-id="1b18b-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="1b18b-115">След това попълнете основния текст, като използвате проектоматериала в секцията "аналитични данни за клиенти" на страницата с правило "алхимията"</span><span class="sxs-lookup"><span data-stu-id="1b18b-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="1b18b-116">Списъците с водещи символи са фини</span><span class="sxs-lookup"><span data-stu-id="1b18b-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="1b18b-117">Номерирани списъци</span><span class="sxs-lookup"><span data-stu-id="1b18b-117">Numbered lists too</span></span>
    1. <span data-ttu-id="1b18b-118">**Получер** и *курсив* са а-ОК</span><span class="sxs-lookup"><span data-stu-id="1b18b-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="1b18b-119">Връзките трябва винаги да бъдат или **"връзки към уеб"/външни** или **Deep-връзки към елементи на потребителския интерфейс**, а не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="1b18b-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="1b18b-120">Картините не се поддържат официално в момента, но са на пътната карта.</span><span class="sxs-lookup"><span data-stu-id="1b18b-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="1b18b-121">И това вече е твърде дълго.</span><span class="sxs-lookup"><span data-stu-id="1b18b-121">And this is really already a bit too long.</span></span> <span data-ttu-id="1b18b-122">Най-добрите практики са около 400 знака---------------------------------</span><span class="sxs-lookup"><span data-stu-id="1b18b-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="1b18b-123">След като съдържанието ви е готово, издърпайте го към живия клон.</span><span class="sxs-lookup"><span data-stu-id="1b18b-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="1b18b-124">След това отидете на [портала за партньори алхимията](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето за URL адрес.</span><span class="sxs-lookup"><span data-stu-id="1b18b-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 