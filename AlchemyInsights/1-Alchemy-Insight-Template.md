---
title: 'същото като името на файла е най-добре [правило #-описание]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939267"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="62ef8-102">Изисква алхимия заглавие H1, H2 на не работят.</span><span class="sxs-lookup"><span data-stu-id="62ef8-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="62ef8-103">Най-добрите практики и насоки за алхимията авторство:</span><span class="sxs-lookup"><span data-stu-id="62ef8-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="62ef8-p101">**Не гнездо алхимия прозрения в папки**- това ще наруши структурата на URL адреса. Ние търсим в това определяне.</span><span class="sxs-lookup"><span data-stu-id="62ef8-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="62ef8-106">Файловете в папката **AlchemyInsights** трябва да има правило ИД и името на правилото от [алхимия партньор портал](https://alchemyportal.azurewebsites.net) в името на файла.</span><span class="sxs-lookup"><span data-stu-id="62ef8-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="62ef8-p102">пример: ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="62ef8-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="62ef8-p103">Използвайте метаданни в горната част на този файл като вашия шаблон. Нищо друго не се изисква.</span><span class="sxs-lookup"><span data-stu-id="62ef8-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="62ef8-111">В [алхимията партньор портал](https://alchemyportal.azurewebsites.net), Навигирайте до раздела **клиент прозрение заглавие:** и използване, че като отправна точка за H1 заглавието за прозрение.</span><span class="sxs-lookup"><span data-stu-id="62ef8-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="62ef8-p104">Алхимия прозрения трябва да имате само един H1 отгоре или те ще бъдат разделени в производството. H2s не правят толкова употреба **смели** или други конвенции да означават отделни раздели.</span><span class="sxs-lookup"><span data-stu-id="62ef8-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="62ef8-114">След това попълнете в основния текст с помощта на проекта материал в раздела клиент прозрения на страницата на алхимията правило</span><span class="sxs-lookup"><span data-stu-id="62ef8-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="62ef8-115">Списъци с водещи символи са добре</span><span class="sxs-lookup"><span data-stu-id="62ef8-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="62ef8-116">Номерирани списъци твърде</span><span class="sxs-lookup"><span data-stu-id="62ef8-116">Numbered lists too</span></span>
    1. <span data-ttu-id="62ef8-117">**Bold** и *курсив* са добре</span><span class="sxs-lookup"><span data-stu-id="62ef8-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="62ef8-118">Връзки винаги трябва да бъде или **"връзки към уеб" / външен** или **дълбоко-връзки към елементи на потребителския интерфейс**, не вътрешни връзки.</span><span class="sxs-lookup"><span data-stu-id="62ef8-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="62ef8-p105">И това наистина вече е малко прекалено дълго. Най-добрата практика е около 400 знака---</span><span class="sxs-lookup"><span data-stu-id="62ef8-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="62ef8-p106">След като вашето съдържание е готов, го дръпнете на живо клон. След това отидете на [алхимията партньор портал](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето url. Уверете се, прозрение прегледани и публикува казва "да" и след това щракнете върху правило за актуализиране. **(Това ще изглежда по-красива в новата версия на портала - освобождаване скоро.)** 
 ![url поле](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="62ef8-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

