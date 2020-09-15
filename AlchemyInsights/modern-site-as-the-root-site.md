---
title: Модерен сайт като главен сайт
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666859"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0aafa-102">Модерен сайт като главен сайт</span><span class="sxs-lookup"><span data-stu-id="0aafa-102">Modern site as root site</span></span>

<span data-ttu-id="0aafa-103">Ние започнахме да внедряваме нова функция, която ще ви помогне да [размените своя класически сайт за главни сайтове с модерен сайт](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="0aafa-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="0aafa-104">Използвайте " [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) ", за да размените местоположението на сайт с друг сайт, докато архивирате първоначалния сайт.</span><span class="sxs-lookup"><span data-stu-id="0aafa-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0aafa-105">Налични и за двата екипа на сайта (не е свързан с група) и комуникационен сайт.</span><span class="sxs-lookup"><span data-stu-id="0aafa-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="0aafa-106">Не изтривайте класическия си главен сайт, за да създадете модерен комуникационен сайт.</span><span class="sxs-lookup"><span data-stu-id="0aafa-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0aafa-107">Това не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0aafa-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="0aafa-108">Изтриването на главния сайт ще направи всички сайтове на SharePoint във вашата организация недостъпни за всички потребители, докато не възстановите сайта или не създадете нов сайт на един и същ URL адрес.</span><span class="sxs-lookup"><span data-stu-id="0aafa-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="0aafa-109">Ще комуникираме с тази функция чрез центъра за съобщения.</span><span class="sxs-lookup"><span data-stu-id="0aafa-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="0aafa-110">Би трябвало да очаквате тази функция да бъде включена в своя клиент скоро.</span><span class="sxs-lookup"><span data-stu-id="0aafa-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0aafa-111">Известни проблеми със смяната на сайтове</span><span class="sxs-lookup"><span data-stu-id="0aafa-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="0aafa-112">Целевият сайт може да върне грешка "не е намерен" (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="0aafa-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0aafa-113">Съдържанието ще трябва да бъде обходено, за да се актуализира индексът за търсене.</span><span class="sxs-lookup"><span data-stu-id="0aafa-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0aafa-114">Тук не се изисква ръчна стъпка, това ще бъде извършено автоматично.</span><span class="sxs-lookup"><span data-stu-id="0aafa-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="0aafa-115">Всичко, което зависи от "статичните" връзки (като файлове за синхронизиране на файлове и OneNote), ще трябва да бъде коригирано ръчно.</span><span class="sxs-lookup"><span data-stu-id="0aafa-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0aafa-116">За да се гарантира, че те все още се асоциират правилно, може да се наложи да бъдат утвърдени сайтовете на Project Server.</span><span class="sxs-lookup"><span data-stu-id="0aafa-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
