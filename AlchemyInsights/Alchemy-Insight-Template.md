---
title: същото като името на файла е най-добро
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664123"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="30d78-102">"Задължително заглавна алхимията H1, H2's не работят."</span><span class="sxs-lookup"><span data-stu-id="30d78-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="30d78-103">Най-добри практики и указания за авторство на алхимията:</span><span class="sxs-lookup"><span data-stu-id="30d78-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="30d78-104">Не **влагайте данни за алхимията в папките**– това ще развали структурата на URL адреса.</span><span class="sxs-lookup"><span data-stu-id="30d78-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="30d78-105">Търсим как да оправим това.</span><span class="sxs-lookup"><span data-stu-id="30d78-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="30d78-106">Файловете в папката **AlchemyInsights** трябва да са с малки имена с тирета за интервали ex.</span><span class="sxs-lookup"><span data-stu-id="30d78-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="30d78-107">***практически указания за разрешаване на конфликт***</span><span class="sxs-lookup"><span data-stu-id="30d78-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="30d78-108">Включете ИД на правилото или ИД на кофа от [портала на партньора в алхимията](https://alchemyportal.azurewebsites.net) в MS. Custom Field.</span><span class="sxs-lookup"><span data-stu-id="30d78-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="30d78-109">ex.</span><span class="sxs-lookup"><span data-stu-id="30d78-109">ex.</span></span> <span data-ttu-id="30d78-110">***MS. по избор: 100021***</span><span class="sxs-lookup"><span data-stu-id="30d78-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="30d78-111">Използвайте останалите метаданни в горния край на този файл като шаблон.</span><span class="sxs-lookup"><span data-stu-id="30d78-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="30d78-112">В [портала за партньори на алхимията](https://alchemyportal.azurewebsites.net)отидете до раздела Заглавие на **клиент Insight:** и използвайте това като отправна точка за своето заглавие H1 за Insight.</span><span class="sxs-lookup"><span data-stu-id="30d78-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="30d78-113">Данни за алхимията трябва да имат само един H1 в горната част или ще се счупят в производството.</span><span class="sxs-lookup"><span data-stu-id="30d78-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="30d78-114">H2s не прави така, че да използва **смели** или други конвенции, за да означава отделни секции.</span><span class="sxs-lookup"><span data-stu-id="30d78-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="30d78-115">След това попълнете основния текст с помощта на проекта за материал в секцията "прозрения за клиенти" на страницата "правило за алхимията"</span><span class="sxs-lookup"><span data-stu-id="30d78-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="30d78-116">Списъците с водещи символи са добре</span><span class="sxs-lookup"><span data-stu-id="30d78-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="30d78-117">Номерирани списъци</span><span class="sxs-lookup"><span data-stu-id="30d78-117">Numbered lists too</span></span>
    1. <span data-ttu-id="30d78-118">**Получер** и *курсив* са-OK</span><span class="sxs-lookup"><span data-stu-id="30d78-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="30d78-119">Връзките винаги трябва да са **"връзки към уеб"/External** или **дълбоки връзки към елементи на потребителския интерфейс**, а не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="30d78-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="30d78-120">Снимките не се поддържат официално в момента, но са в пътната карта.</span><span class="sxs-lookup"><span data-stu-id="30d78-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="30d78-121">А това вече е твърде много.</span><span class="sxs-lookup"><span data-stu-id="30d78-121">And this is really already a bit too long.</span></span> <span data-ttu-id="30d78-122">Най-добрата практика е около 400 знака---------------------------------</span><span class="sxs-lookup"><span data-stu-id="30d78-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="30d78-123">След като съдържанието ви е готово, го издърпайте към клона на живо.</span><span class="sxs-lookup"><span data-stu-id="30d78-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="30d78-124">След това отидете на [портала за партньори на алхимията](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето за URL адрес.</span><span class="sxs-lookup"><span data-stu-id="30d78-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 