---
title: Записване на сайт или списък като шаблон
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2019
ms.locfileid: "31043994"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="82d9e-102">Записване на сайт или списък като шаблон</span><span class="sxs-lookup"><span data-stu-id="82d9e-102">Save site or list as a template</span></span>

<span data-ttu-id="82d9e-103">Шаблони за сайтове на SharePoint са предварително създадени дефиниции, предназначени около на дадена бизнес нужда.</span><span class="sxs-lookup"><span data-stu-id="82d9e-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="82d9e-104">За повече информация вижте [използване на шаблони за създаване на различни видове на сайтове на SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="82d9e-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="82d9e-105">Ето някои често срещани проблеми/решения по отношение на спестяване на сайт или списък като шаблон в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="82d9e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="82d9e-106">**Запиши сайт/списък храм копче е не наличен или липсва**.</span><span class="sxs-lookup"><span data-stu-id="82d9e-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="82d9e-107">Администраторите ще трябва да разрешите потребителски скрипт да разрешите шаблона функции.</span><span class="sxs-lookup"><span data-stu-id="82d9e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="82d9e-108">За подробни стъпки, примери и съображения вижте [Разрешаване или предотвратяване на потребителски скрипт](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="82d9e-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="82d9e-109">Запиши сайта като шаблон команда не се поддържа и може да причини проблеми на сайтове, които използват SharePoint Server публикуване инфраструктура.</span><span class="sxs-lookup"><span data-stu-id="82d9e-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


**<span data-ttu-id="82d9e-110">Шаблонът на сайта не може да бъде създадена или не работи правилно</span><span class="sxs-lookup"><span data-stu-id="82d9e-110">The site template cannot be created or does not work correctly</span></span>**

- <span data-ttu-id="82d9e-111">Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и няма да се активира.</span><span class="sxs-lookup"><span data-stu-id="82d9e-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="82d9e-112">Ако функцията не е достъпна за да активирате в текущата колекция от сайтове, можете да използвате шаблона за сайт за създаване на сайт.</span><span class="sxs-lookup"><span data-stu-id="82d9e-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="82d9e-113">Проверете дали някакви списъци или библиотеки надвишават [Праг на списъчен изглед лимит](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) от 5000 позиции, тъй като това може да блокира създаването на шаблон на сайт.</span><span class="sxs-lookup"><span data-stu-id="82d9e-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="82d9e-114">Сайтът може да се използва твърде много ресурси и следователно шаблона сайт надвишава ограничението за 50 мегабайта (МБ).</span><span class="sxs-lookup"><span data-stu-id="82d9e-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="82d9e-115">Има проблеми при показването на данни от списък, който използва справочна колона.</span><span class="sxs-lookup"><span data-stu-id="82d9e-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="82d9e-116">За повече информация вижте [, генерирано от шаблон на списък не се показва данни от списъка с правилното търсене в SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="82d9e-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="82d9e-117">За по-подробна информация по общи проблеми и решения, моля позоваване, [Създаване и използване на сайта шаблони](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="82d9e-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

