---
title: Заявка за Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974181"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="815b4-102">Заявка за Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="815b4-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="815b4-103">Тази тема може да се приложи и за разработчиците, които все още използват Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="815b4-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="815b4-104">Все пак **настоятелно** се препоръчва да използвате Microsoft Graph за всички сценарии на вашия указател, самоличност и управление на достъпа.</span><span class="sxs-lookup"><span data-stu-id="815b4-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="815b4-105">**Проблеми при удостоверяване или упълномощаване**</span><span class="sxs-lookup"><span data-stu-id="815b4-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="815b4-106">Ако вашето приложение не е в **състояние да получи маркери** , за да се обадите на Microsoft Graph, изберете **проблем** , за да получите по-конкретна помощ и поддръжка на тази тема.</span><span class="sxs-lookup"><span data-stu-id="815b4-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="815b4-107">Ако вашето приложение **получава грешки за удостоверяване на 401 или 403** , когато се обаждате на Microsoft Graph, изберете категорията API за **получаване на отказан достъп (разрешение)** Microsoft Graph, за да получите по-конкретна помощ и поддръжка на тази тема.</span><span class="sxs-lookup"><span data-stu-id="815b4-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="815b4-108">**Искам да използвам Microsoft Graph, но не знам откъде да започна**</span><span class="sxs-lookup"><span data-stu-id="815b4-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="815b4-109">За да научите повече за Microsoft Graph, вижте:</span><span class="sxs-lookup"><span data-stu-id="815b4-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="815b4-110">Общ преглед на Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="815b4-111">Обзор на управлението на самоличността и достъпа в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="815b4-112">Първи стъпки в създаването на приложения на Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="815b4-113">**Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демонстрация</span><span class="sxs-lookup"><span data-stu-id="815b4-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="815b4-114">**Искам да използвам Microsoft Graph, но поддържа ли API за v 1,0 директорията, от която се нуждая?**</span><span class="sxs-lookup"><span data-stu-id="815b4-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="815b4-115">Microsoft Graph представлява препоръчвания API за адресна книга, самоличност и управление на достъпа.</span><span class="sxs-lookup"><span data-stu-id="815b4-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="815b4-116">Но все още има някои пропуски между това, което е възможно в Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="815b4-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="815b4-117">Прегледайте статиите по-долу, които осветяват най-актуалните разлики, за да ви помогнат по ваш избор:</span><span class="sxs-lookup"><span data-stu-id="815b4-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="815b4-118">Разлики между типовете ресурси между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="815b4-119">Разлики между свойствата между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="815b4-120">Разлики в методите между Azure AD и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="815b4-121">**Когато задавам заявка за *потребителския* обект, много от свойствата му липсват**</span><span class="sxs-lookup"><span data-stu-id="815b4-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="815b4-122">`GET https://graph.microsoft.com/v1.0/users` връща само 11 свойства, тъй като Microsoft Graph автоматично избира набор от *потребителски* свойства по подразбиране, за да се върне.</span><span class="sxs-lookup"><span data-stu-id="815b4-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="815b4-123">Ако имате нужда от други *потребителски* свойства, използвайте $Select, за да изберете свойствата, от които се нуждае вашата заявка.</span><span class="sxs-lookup"><span data-stu-id="815b4-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="815b4-124">Изпробвайте го първо в **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="815b4-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="815b4-125">**Някои потребителски стойности на свойства са *NULL* въпреки че знам, че са зададени**</span><span class="sxs-lookup"><span data-stu-id="815b4-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="815b4-126">Най-вероятно обяснение е, че приложението е дало на *потребителя. ReadBasic. All* разрешение.</span><span class="sxs-lookup"><span data-stu-id="815b4-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="815b4-127">Това позволява на приложението да прочете ограничен набор от потребителски свойства, като връща всички други свойства като Null дори ако са били предварително зададени.</span><span class="sxs-lookup"><span data-stu-id="815b4-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="815b4-128">Опитайте да отпуснете приложението *User. read. All* разрешение вместо това.</span><span class="sxs-lookup"><span data-stu-id="815b4-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="815b4-129">За повече информация вижте [потребителски разрешения за Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="815b4-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="815b4-130">**Имам проблеми с използването на параметри на заявката OData за филтриране на данни в моите искания**</span><span class="sxs-lookup"><span data-stu-id="815b4-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="815b4-131">Докато Microsoft Graph поддържа широк диапазон от параметри на заявката за OData, много от тези параметри не се поддържат напълно от справочните услуги (ресурси, които се наследяват от *directoryObject*) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="815b4-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="815b4-132">Същите ограничения, които присъстваха в Azure AD Graph, продължават по-голямата част от Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="815b4-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="815b4-133">**Не се поддържа**: $count, $search и $Filter върху стойности *NULL* или *NOT NULL*</span><span class="sxs-lookup"><span data-stu-id="815b4-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="815b4-134">**Не се поддържа**: $Filter за определени свойства (Вижте теми за ресурси, в които свойствата могат да се филтрират)</span><span class="sxs-lookup"><span data-stu-id="815b4-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="815b4-135">**Не се поддържа**: страниране, филтриране и сортиране едновременно</span><span class="sxs-lookup"><span data-stu-id="815b4-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="815b4-136">**Не се поддържа**: филтриране по релация.</span><span class="sxs-lookup"><span data-stu-id="815b4-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="815b4-137">Например – Намерете всички членове на инженерната група, които са в Обединеното кралство.</span><span class="sxs-lookup"><span data-stu-id="815b4-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="815b4-138">**Частична поддръжка**: $orderby на *потребител* (само за displayName и userPrincipalName) и *Група*</span><span class="sxs-lookup"><span data-stu-id="815b4-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="815b4-139">**Частична поддръжка**: $Filter (поддържа само *EQ*, *startswith* *или*, *и* и ограничава *всякакви*) поддръжка $expand (разширяването на релациите на един обект връща всички релации, но разширяването на колекция от релации на обекти е ограничено)</span><span class="sxs-lookup"><span data-stu-id="815b4-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="815b4-140">За повече информация вижте [Персонализиране на отговори с параметри на заявка](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="815b4-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="815b4-141">**API-то, на което се обаждам, не работи – къде мога да направя още тестване?**</span><span class="sxs-lookup"><span data-stu-id="815b4-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="815b4-142">**Microsoft Graph Explorer** – Тествайте API за Microsoft Graph в своя клиент или клиент за демо и също така разгледайте **примерните заявки** в Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="815b4-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="815b4-143">**Когато имам заявка за данни, изглежда, че получавам незавършен набор данни обратно**</span><span class="sxs-lookup"><span data-stu-id="815b4-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="815b4-144">Ако задавате заявка за събиране (като *потребители*), Microsoft Graph използва ограничения за страниците на сървъра, така че резултатите винаги да се връщат с размер на страницата по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="815b4-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="815b4-145">Приложението ви трябва винаги да очаква да се изпраща на страница чрез колекции, върнати от услугата.</span><span class="sxs-lookup"><span data-stu-id="815b4-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="815b4-146">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="815b4-146">For more information, see:</span></span>

- [<span data-ttu-id="815b4-147">Най-добри практики за Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="815b4-148">Пейджинг данни за Microsoft Graph във вашето приложение</span><span class="sxs-lookup"><span data-stu-id="815b4-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="815b4-149">**Приложението ми е твърде бавно и все още не може да се регулира. Какви подобрения мога да направя?**</span><span class="sxs-lookup"><span data-stu-id="815b4-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="815b4-150">В зависимост от сценария ви има редица различни опции на ваше разположение, за да направите приложението си по-съобразно и в някои случаи по-малко податливи на ограничаване на услугата (когато провеждате твърде много обаждания).</span><span class="sxs-lookup"><span data-stu-id="815b4-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="815b4-151">За да научите повече, вижте:</span><span class="sxs-lookup"><span data-stu-id="815b4-151">To learn more, see:</span></span>

- [<span data-ttu-id="815b4-152">Най-добри практики за Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="815b4-153">Изисквания за дозиране</span><span class="sxs-lookup"><span data-stu-id="815b4-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="815b4-154">Следене на промените чрез Делта заявка</span><span class="sxs-lookup"><span data-stu-id="815b4-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="815b4-155">Получаване на известие за промените чрез webhooks</span><span class="sxs-lookup"><span data-stu-id="815b4-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="815b4-156">Ограничаване на указания</span><span class="sxs-lookup"><span data-stu-id="815b4-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="815b4-157">**Къде мога да намеря повече информация за грешки и известни проблеми?**</span><span class="sxs-lookup"><span data-stu-id="815b4-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="815b4-158">Информация за отговора на грешката на Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="815b4-159">Известни проблеми с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="815b4-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="815b4-160">**Къде мога да проверя състоянието на наличност и свързване на услугата?**</span><span class="sxs-lookup"><span data-stu-id="815b4-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="815b4-161">Наличността на услугата и свързването на основните услуги, които са достъпни чрез Microsoft Graph, могат да окажат влияние върху цялостната достъпност и производителност на Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="815b4-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="815b4-162">За изправност на услугата Azure Active Directory Проверете състоянието на услугите за **защита + самоличност** , показани в [страницата за състояние на Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="815b4-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="815b4-163">За услуги на Office, които допринасят за Microsoft Graph, проверете състоянието на услугите, които са посочени в [таблото за изправност на услугите на Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="815b4-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
