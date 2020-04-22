---
title: същото като името на файла е най-добре
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
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676522"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="dacbe-102">Изискван Алхимия H1, H2's не работи.</span><span class="sxs-lookup"><span data-stu-id="dacbe-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="dacbe-103">Най-добри практики и насоки за авторство на Алхимия:</span><span class="sxs-lookup"><span data-stu-id="dacbe-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="dacbe-104">**Не внедри Alchemy Insights в папки**- това ще наруши структурата на URL адреса.</span><span class="sxs-lookup"><span data-stu-id="dacbe-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="dacbe-105">Ще го оправим.</span><span class="sxs-lookup"><span data-stu-id="dacbe-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="dacbe-106">Файлове в папката **AlchemyInsights** трябва да имат малки имена на файлове с тире за интервали ех.</span><span class="sxs-lookup"><span data-stu-id="dacbe-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="dacbe-107">***как да се разреши задържане на съдебния процес***.</span><span class="sxs-lookup"><span data-stu-id="dacbe-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="dacbe-108">Включете ИД на правилото или ИД на кофа та от [портала на алхимията в](https://alchemyportal.azurewebsites.net) полето ms.custom.</span><span class="sxs-lookup"><span data-stu-id="dacbe-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="dacbe-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="dacbe-109">ex.</span></span> <span data-ttu-id="dacbe-110">***мс.поизбор: 100021***</span><span class="sxs-lookup"><span data-stu-id="dacbe-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="dacbe-111">Използвайте останалите метаданни в горната част на този файл като шаблон.</span><span class="sxs-lookup"><span data-stu-id="dacbe-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="dacbe-112">В [портала За Партньори алхимията](https://alchemyportal.azurewebsites.net)навигирайте надолу до секцията **Заглавие на Клиента:** и я използвайте като отправна точка за вашето Заглавие H1 за прозрението.</span><span class="sxs-lookup"><span data-stu-id="dacbe-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="dacbe-113">Alchemy Insights ТРЯБВА да има само един H1 на върха или те ще се счупи в производството.</span><span class="sxs-lookup"><span data-stu-id="dacbe-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="dacbe-114">H2 s не прави така, така че използвайте **смели** или други конвенции, за да означаваотделни раздели.</span><span class="sxs-lookup"><span data-stu-id="dacbe-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="dacbe-115">След това попълнете основния текст с помощта на чернова на материала в секцията "Данни за клиента" на страницата "Правило за Алхимия"</span><span class="sxs-lookup"><span data-stu-id="dacbe-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="dacbe-116">Списъците с водещи символи са добре</span><span class="sxs-lookup"><span data-stu-id="dacbe-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="dacbe-117">Номерирани списъци също</span><span class="sxs-lookup"><span data-stu-id="dacbe-117">Numbered lists too</span></span>
    1. <span data-ttu-id="dacbe-118">**Получер** и *курсив* са a-ок</span><span class="sxs-lookup"><span data-stu-id="dacbe-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="dacbe-119">Връзките винаги трябва да са **"връзки към уеб"/външни** ИЛИ **дълбоки връзки към елементи на потребителския интерфейс,** а не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="dacbe-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="dacbe-120">Снимките не се поддържат официално в момента, но са на пътната карта.</span><span class="sxs-lookup"><span data-stu-id="dacbe-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="dacbe-121">И това вече е твърде дълго.</span><span class="sxs-lookup"><span data-stu-id="dacbe-121">And this is really already a bit too long.</span></span> <span data-ttu-id="dacbe-122">Най-добрата практика е около 400 знака ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="dacbe-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="dacbe-123">След като съдържанието ви е готово, изтеглете го към жив клон.</span><span class="sxs-lookup"><span data-stu-id="dacbe-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="dacbe-124">След това отидете на [портала на партньора на Алхимията](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето URL.</span><span class="sxs-lookup"><span data-stu-id="dacbe-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 