---
title: Създаване на сайт в SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514987"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="b4fca-102">Създаване на сайтове на SharePoint с помощта на шаблони</span><span class="sxs-lookup"><span data-stu-id="b4fca-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="b4fca-103">Шаблони за сайтове на SharePoint са предварително създадени дефиниции, предназначени около на дадена бизнес нужда.</span><span class="sxs-lookup"><span data-stu-id="b4fca-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="b4fca-104">За повече информация вижте [използване на шаблони за създаване на различни видове на сайтове на SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="b4fca-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="b4fca-105">Ето някои често срещани проблеми/решения по отношение на спестяване на сайт или списък като шаблон в Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="b4fca-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="b4fca-106">**Запиши сайт/списък шаблон бутон не е наличен или липсва**</span><span class="sxs-lookup"><span data-stu-id="b4fca-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="b4fca-107">Администраторите ще трябва да разрешите потребителски скрипт да разрешите шаблона функции.</span><span class="sxs-lookup"><span data-stu-id="b4fca-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="b4fca-108">За подробни стъпки Вижте примери и съображения</span><span class="sxs-lookup"><span data-stu-id="b4fca-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="b4fca-109">Разрешаване или предотвратяване на потребителски скрипт</span><span class="sxs-lookup"><span data-stu-id="b4fca-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="b4fca-110">Запиши сайта като шаблон команда не се поддържа и може да причини проблеми на сайтове, които използват SharePoint Server публикуване инфраструктура.</span><span class="sxs-lookup"><span data-stu-id="b4fca-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="b4fca-111">**Шаблонът на сайта не може да бъде създадена или не работи правилно**</span><span class="sxs-lookup"><span data-stu-id="b4fca-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="b4fca-112">Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и няма да се активира.</span><span class="sxs-lookup"><span data-stu-id="b4fca-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="b4fca-113">Ако функцията не е достъпна за да активирате в текущата колекция от сайтове, можете да използвате шаблона за сайт за създаване на сайт.</span><span class="sxs-lookup"><span data-stu-id="b4fca-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="b4fca-114">Проверете дали някакви списъци или библиотеки надвишават [Праг на списъчен изглед лимит](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) от 5000 позиции, тъй като това може да блокира създаването на шаблон на сайт.</span><span class="sxs-lookup"><span data-stu-id="b4fca-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="b4fca-115">Сайтът може да се използва твърде много ресурси и следователно шаблона на сайта надхвърля 50 MB граница.</span><span class="sxs-lookup"><span data-stu-id="b4fca-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="b4fca-116">Има проблеми при показването на данни от списък, който използва справочна колона.</span><span class="sxs-lookup"><span data-stu-id="b4fca-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="b4fca-117">За повече информация вижте [, генерирано от шаблон на списък не се показва данни от списъка с правилното търсене в SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="b4fca-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="b4fca-118">За по-подробна информация по общи проблеми и решения моля проверете [Създаване и използване на сайта шаблони](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="b4fca-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



