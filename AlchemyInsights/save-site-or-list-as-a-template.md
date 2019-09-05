---
title: Записване на сайт или списък като шаблон
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752021"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="cbc1d-102">Записване на сайт или списък като шаблон</span><span class="sxs-lookup"><span data-stu-id="cbc1d-102">Save site or list as a template</span></span>

<span data-ttu-id="cbc1d-103">Шаблоните за сайтове на SharePoint са предварително построени дефиниции, проектирани около конкретна бизнес потребност.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="cbc1d-104">За повече информация вижте [използване на шаблони за създаване на различни видове сайтове на SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="cbc1d-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="cbc1d-105">Ето някои често срещани проблеми/решения по отношение на записването на сайт или списък като шаблон в SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="cbc1d-106">**Бутонът за запис на шаблон за сайт/списък не е наличен или липсва**.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="cbc1d-107">Администраторите ще трябва да разрешат персонализирания скрипт, за да разрешат функциите на шаблона.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="cbc1d-108">За подробни стъпки, примери и съображения вижте [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="cbc1d-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="cbc1d-109">Командата за записване на сайта като шаблон не се поддържа и може да доведе до проблеми на сайтове, използващи инфраструктура за публикуване на SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="cbc1d-110">**Шаблонът на сайта не може да бъде създаден или не работи правилно**</span><span class="sxs-lookup"><span data-stu-id="cbc1d-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="cbc1d-111">Може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) на шаблона и да не се активира.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="cbc1d-112">Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона на сайта, за да създадете сайт.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="cbc1d-113">Проверете дали някои списъци или библиотеки надхвърлят [прага за ограничаване на списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) на 5000 елемента, тъй като това може да блокира създаването на шаблон на сайт.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="cbc1d-114">Сайтът може да използва твърде много ресурси и следователно шаблонът на сайта надвишава ограничението от 50 мегабайта (МБ).</span><span class="sxs-lookup"><span data-stu-id="cbc1d-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="cbc1d-115">Има проблеми с показването на данни от списък, който използва справочна колона.</span><span class="sxs-lookup"><span data-stu-id="cbc1d-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="cbc1d-116">За повече информация вижте [шаблон генериран списък не показва данни от правилния списък за търсене в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="cbc1d-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="cbc1d-117">За по-подробна информация относно често срещани проблеми и решения, моля препратка, [Създаване и използване на шаблони за сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="cbc1d-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

