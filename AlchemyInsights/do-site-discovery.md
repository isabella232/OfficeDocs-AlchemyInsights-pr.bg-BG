---
title: Откриване на сайт
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692533"
---
# <a name="do-site-discovery"></a><span data-ttu-id="8739a-102">Откриване на сайт</span><span class="sxs-lookup"><span data-stu-id="8739a-102">Do site discovery</span></span>

<span data-ttu-id="8739a-103">Ако вашата организация все още използва стари уеб приложения и планира да използва режима на Internet Explorer (което повечето клиенти имат), трябва да направите допълнително откриване на сайта.</span><span class="sxs-lookup"><span data-stu-id="8739a-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="8739a-104">**Вече сте разположили по-стара версия на Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="8739a-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="8739a-105">Ако вече сте конфигурирали вашия списък с корпоративен сайт за работа с наследени версии на Microsoft Edge, откриването на сайта е почти готово.</span><span class="sxs-lookup"><span data-stu-id="8739a-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="8739a-106">Едно нещо, което може да се наложи да направите, е да добавите неутрални сайтове.</span><span class="sxs-lookup"><span data-stu-id="8739a-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="8739a-107">Неутралните сайтове обикновено са сайтовете, които предоставят еднократна идентификация (SSO).</span><span class="sxs-lookup"><span data-stu-id="8739a-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="8739a-108">Ако отидете в неутрален сайт от Microsoft Edge, след което искате да останете в Microsoft Edge за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="8739a-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="8739a-109">Ако отидете в неутрален сайт в режим на Internet Explorer, трябва да останете в режима на Internet Explorer, за да удостоверите самоличността си.</span><span class="sxs-lookup"><span data-stu-id="8739a-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="8739a-110">Можете да идентифицирате всеки див или друг неутрален сайт, който използвате, и да ги добавите към вашия списък с корпоративни сайтове.</span><span class="sxs-lookup"><span data-stu-id="8739a-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="8739a-111">**Internet Explorer е вашият браузър по подразбиране**</span><span class="sxs-lookup"><span data-stu-id="8739a-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="8739a-112">Ако използвате само Internet Explorer сега, е възможно да не знаете кои сайтове са надстроени до съвременните уеб стандарти и което все още изисква Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8739a-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="8739a-113">Ще искате да търсите и да добавяте тези сайтове към списъка с корпоративни сайтове, така че да можете да използвате режима на Internet Explorer само за тези сайтове.</span><span class="sxs-lookup"><span data-stu-id="8739a-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="8739a-114">[Откритието Enterprise Site](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) открива сайтовете, които може да са необходими за режима на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8739a-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="8739a-115">В Windows 10, Windows 8,1 или Windows 7 можете да събирате данни на компютри, на които се изпълнява Windows Internet Explorer 8 чрез Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="8739a-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="8739a-116">**Анализиране на данни**</span><span class="sxs-lookup"><span data-stu-id="8739a-116">**Analyze the data**</span></span>

<span data-ttu-id="8739a-117">След като съберете данни за сайта, ви препоръчваме следния процес от четири стъпки за анализиране на данните:</span><span class="sxs-lookup"><span data-stu-id="8739a-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="8739a-118">Сортирайте данните по домейн и след това чрез URL адрес.</span><span class="sxs-lookup"><span data-stu-id="8739a-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="8739a-119">Определете границите на дадено приложение, за да конфигурирате за режим на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8739a-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="8739a-120">Искате да включите всички сайтове и уеб контроли, които определят приложението, но не искате да включвате допълнителни сайтове и контроли.</span><span class="sxs-lookup"><span data-stu-id="8739a-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="8739a-121">Някои сайтове може да са толкова прости, *https://contoso.com/app1* докато други може да изискват от вас да дефинирате множество сайтове и страници.</span><span class="sxs-lookup"><span data-stu-id="8739a-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="8739a-122">Изпробвайте приложението, за да се уверите, че не работи по този език.</span><span class="sxs-lookup"><span data-stu-id="8739a-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="8739a-123">Много сайтове ще ви предложат модерно съдържание, когато откриват модерен браузър и предлагат само наследени съдържание, когато откриват Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8739a-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="8739a-124">Добавете приложението към вашия списък с корпоративен сайт, ако то не е изпробвано.</span><span class="sxs-lookup"><span data-stu-id="8739a-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="8739a-125">Като най-добра практика групирайте всички сайтове, които съдържат приложение.</span><span class="sxs-lookup"><span data-stu-id="8739a-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="8739a-126">По този начин, когато надстроите приложение, е по-лесно да премахнете целия сайт от режим на Internet Explorer и да започнете да използвате модерен браузър за това приложение.</span><span class="sxs-lookup"><span data-stu-id="8739a-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="8739a-127">Когато сте готови с откриването на сайта и сте анализирали данните, сте готови да започнете да преглеждате стратегията си за канала.</span><span class="sxs-lookup"><span data-stu-id="8739a-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

