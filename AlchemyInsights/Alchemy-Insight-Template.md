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
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762054"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d9447-102">Изисква алхимия заглавие H1, H2 на не работят.</span><span class="sxs-lookup"><span data-stu-id="d9447-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d9447-103">Най-добрите практики и насоки за алхимията авторство:</span><span class="sxs-lookup"><span data-stu-id="d9447-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d9447-104">**Не гнездо алхимия прозрения в папки**- това ще наруши структурата на URL адреса.</span><span class="sxs-lookup"><span data-stu-id="d9447-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d9447-105">Ние търсим в това определяне.</span><span class="sxs-lookup"><span data-stu-id="d9447-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d9447-106">Файловете в папката **AlchemyInsights** трябва да имат малки файлове с тирета за пространства ex.</span><span class="sxs-lookup"><span data-stu-id="d9447-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="d9447-107">***как-към-разрешаване--задържане***.</span><span class="sxs-lookup"><span data-stu-id="d9447-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="d9447-108">Включва ИД на правилото за ИД или кофа от [алхимия партньор портал](https://alchemyportal.azurewebsites.net) в областта на ms.custom.</span><span class="sxs-lookup"><span data-stu-id="d9447-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="d9447-109">ех.</span><span class="sxs-lookup"><span data-stu-id="d9447-109">ex.</span></span> <span data-ttu-id="d9447-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="d9447-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="d9447-111">Използвайте останалата част от метаданните в горната част на този файл като вашия шаблон.</span><span class="sxs-lookup"><span data-stu-id="d9447-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="d9447-112">В [алхимията партньор портал](https://alchemyportal.azurewebsites.net), Навигирайте до раздела **клиент прозрение заглавие:** и използване, че като отправна точка за H1 заглавието за прозрение.</span><span class="sxs-lookup"><span data-stu-id="d9447-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d9447-113">Алхимия прозрения трябва да имате само един H1 отгоре или те ще бъдат разделени в производството.</span><span class="sxs-lookup"><span data-stu-id="d9447-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d9447-114">H2s не правят толкова употреба **смели** или други конвенции да означават отделни раздели.</span><span class="sxs-lookup"><span data-stu-id="d9447-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d9447-115">След това попълнете в основния текст с помощта на проекта материал в раздела клиент прозрения на страницата на алхимията правило</span><span class="sxs-lookup"><span data-stu-id="d9447-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d9447-116">Списъци с водещи символи са добре</span><span class="sxs-lookup"><span data-stu-id="d9447-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d9447-117">Номерирани списъци твърде</span><span class="sxs-lookup"><span data-stu-id="d9447-117">Numbered lists too</span></span>
    1. <span data-ttu-id="d9447-118">**Bold** и *курсив* са добре</span><span class="sxs-lookup"><span data-stu-id="d9447-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d9447-119">Връзки винаги трябва да бъде или **"връзки към уеб" / външен** или **дълбоко-връзки към елементи на потребителския интерфейс**, не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="d9447-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="d9447-120">Снимки не са официално се поддържа в този момент, но това е на пътната карта.</span><span class="sxs-lookup"><span data-stu-id="d9447-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="d9447-121">И това наистина вече е малко прекалено дълго.</span><span class="sxs-lookup"><span data-stu-id="d9447-121">And this is really already a bit too long.</span></span> <span data-ttu-id="d9447-122">Най-добрата практика е около 400 знака---</span><span class="sxs-lookup"><span data-stu-id="d9447-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d9447-123">След като вашето съдържание е готов, го дръпнете на живо клон.</span><span class="sxs-lookup"><span data-stu-id="d9447-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d9447-124">След това отидете на [алхимията партньор портал](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето url.</span><span class="sxs-lookup"><span data-stu-id="d9447-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="d9447-125">М</span><span class="sxs-lookup"><span data-stu-id="d9447-125">M</span></span>