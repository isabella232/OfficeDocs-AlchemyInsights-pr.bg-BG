---
title: като името на файла е най-добре
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750959"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0d68e-102">"Необходим Алхимия H1, H2 не работи."</span><span class="sxs-lookup"><span data-stu-id="0d68e-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="0d68e-103">Най-добри практики и насоки за автори на Алхимия:</span><span class="sxs-lookup"><span data-stu-id="0d68e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0d68e-104">**Не nest Alchemy Insights в папки**- това ще наруши структурата на URL.</span><span class="sxs-lookup"><span data-stu-id="0d68e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0d68e-105">Ще го оправим.</span><span class="sxs-lookup"><span data-stu-id="0d68e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0d68e-106">Файловете в папката **AlchemyInsights** трябва да имат малки имена на файлове с тирета за интервали ex.</span><span class="sxs-lookup"><span data-stu-id="0d68e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0d68e-107">***как да се даде възможност за задържане на съдебни***</span><span class="sxs-lookup"><span data-stu-id="0d68e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0d68e-108">Включете ИД на правило или ИД на картон от портала на [партньора на Alchemy](https://alchemyportal.azurewebsites.net) в полето ms.custom.</span><span class="sxs-lookup"><span data-stu-id="0d68e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0d68e-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="0d68e-109">ex.</span></span> <span data-ttu-id="0d68e-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0d68e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0d68e-111">Използвайте останалата част от метаданните в горната част на този файл като шаблон.</span><span class="sxs-lookup"><span data-stu-id="0d68e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0d68e-112">В портала за [партньори на Alchemy](https://alchemyportal.azurewebsites.net)навигирайте до секцията **"Заглавие на Customer Insight"** и го използвайте като отправна точка за заглавието на H1 за статистиката.</span><span class="sxs-lookup"><span data-stu-id="0d68e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0d68e-113">Alchemy Insights трябва да има само един H1 в горната част или те ще се счупят в производството.</span><span class="sxs-lookup"><span data-stu-id="0d68e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0d68e-114">H2s не правят така, че използват **смели** или други конвенции, за да означават отделни секции.</span><span class="sxs-lookup"><span data-stu-id="0d68e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0d68e-115">След това попълнете основния текст, като използвате черновата в раздел "Статистика на клиентите" на страницата с правила на Alchemy</span><span class="sxs-lookup"><span data-stu-id="0d68e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0d68e-116">Списъците с куршуми са добре</span><span class="sxs-lookup"><span data-stu-id="0d68e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0d68e-117">Номерирани списъци също</span><span class="sxs-lookup"><span data-stu-id="0d68e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0d68e-118">**Смели** и *курсив* са а-ок</span><span class="sxs-lookup"><span data-stu-id="0d68e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0d68e-119">Връзките трябва винаги да бъдат **или "връзки към уеб"/външни** или **дълбоки връзки към елементи на потребителския интерфейс,** а не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="0d68e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0d68e-120">В момента снимките не се поддържат официално, но са в пътната карта.</span><span class="sxs-lookup"><span data-stu-id="0d68e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0d68e-121">И това наистина е доста дълго.</span><span class="sxs-lookup"><span data-stu-id="0d68e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0d68e-122">Най-добрата практика е около 400 знака ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="0d68e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0d68e-123">След като съдържанието ви е готово, го издърпайте към живия клон.</span><span class="sxs-lookup"><span data-stu-id="0d68e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0d68e-124">След това отидете на [alchemy партньор портал](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето URL.</span><span class="sxs-lookup"><span data-stu-id="0d68e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 