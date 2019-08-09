---
title: Модерен сайт като главния сайт
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269365"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="45f21-102">Модерен сайт като главния сайт</span><span class="sxs-lookup"><span data-stu-id="45f21-102">Modern site as root site</span></span>

<span data-ttu-id="45f21-103">Ние са започнали да внедряването на нова функция, която ще ви позволи да сменяте вашия класически сайт корен сайт с модерен сайт.</span><span class="sxs-lookup"><span data-stu-id="45f21-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="45f21-104">Използвайте [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) да сменяте местоположението на един сайт с друг сайт при архивирането на оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="45f21-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="45f21-105">Налични за екипен сайт (не е свързан към група) и комуникация сайт.</span><span class="sxs-lookup"><span data-stu-id="45f21-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="45f21-106">Не изтривайте сайта си класически корен да се създаде сайт на модерната комуникация.</span><span class="sxs-lookup"><span data-stu-id="45f21-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="45f21-107">Това не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="45f21-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="45f21-108">Изтриването на главния сайт ще направи всички SharePoint сайтове във вашата организация недостъпни за всички потребители, докато възстанови сайта или създаване на нов сайт на същия URL адрес.</span><span class="sxs-lookup"><span data-stu-id="45f21-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="45f21-109">Ние ще се общува тази функция чрез център за съобщения.</span><span class="sxs-lookup"><span data-stu-id="45f21-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="45f21-110">Можете да очаквате тази функция да бъде включена в си наемател скоро.</span><span class="sxs-lookup"><span data-stu-id="45f21-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="45f21-111">Известни проблеми с swapping сайтове</span><span class="sxs-lookup"><span data-stu-id="45f21-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="45f21-112">Целта на сайта може да се върне "не е намерена" грешка (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="45f21-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="45f21-113">Съдържанието ще трябва да бъде обходен отново да актуализирате индекса за търсене.</span><span class="sxs-lookup"><span data-stu-id="45f21-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="45f21-114">Там не е ръчно стъпка изисква тук, това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="45f21-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="45f21-115">Всичко зависи от "статичен" връзки (например файл синхронизация и OneNote файлове) ще трябва да бъдат коригирани ръчно.</span><span class="sxs-lookup"><span data-stu-id="45f21-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="45f21-116">Проект сървър сайтове може да се наложи да се проверяват, за да се гарантира, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="45f21-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
