---
title: Създаване на сайт в SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770412"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="82c6b-102">Създаване на сайтове на SharePoint с помощта на шаблони</span><span class="sxs-lookup"><span data-stu-id="82c6b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="82c6b-103">Възможността за записване на сайт като шаблон не се поддържа от модерна комуникация или team sites.</span><span class="sxs-lookup"><span data-stu-id="82c6b-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="82c6b-104">За повече информация относно използването на шаблони вижте [Записване, изтегляне и качване на сайт на SharePoint като шаблон](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="82c6b-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="82c6b-105">Ето някои често срещани проблеми/решения относно Записване на сайт или списък като шаблон в Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="82c6b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="82c6b-106">**Бутонът за запазване на шаблона за сайт/списък не е наличен или липсващ**</span><span class="sxs-lookup"><span data-stu-id="82c6b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="82c6b-107">Администраторите ще трябва да позволи персонализиран скрипт, за да активирате функциите на шаблона.</span><span class="sxs-lookup"><span data-stu-id="82c6b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="82c6b-108">За подробни стъпки, примери и съображения вж.</span><span class="sxs-lookup"><span data-stu-id="82c6b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="82c6b-109">Разрешаване или предотвратяване на персонализиран скрипт</span><span class="sxs-lookup"><span data-stu-id="82c6b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="82c6b-110">Запиши сайта като шаблон командата не се поддържа и може да предизвика проблеми на сайтове, които използват sharePoint Server публикуване инфраструктура.</span><span class="sxs-lookup"><span data-stu-id="82c6b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="82c6b-111">**Шаблонът на сайта не може да бъде създаден или не работи правилно**</span><span class="sxs-lookup"><span data-stu-id="82c6b-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="82c6b-112">Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не се активира.</span><span class="sxs-lookup"><span data-stu-id="82c6b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="82c6b-113">Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона на сайта за създаване на сайт.</span><span class="sxs-lookup"><span data-stu-id="82c6b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="82c6b-114">Проверете дали списъците или библиотеките надвишават прага на ограничението за [списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) от 5000 елемента, тъй като това може да блокира създаването на шаблон на сайт.</span><span class="sxs-lookup"><span data-stu-id="82c6b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="82c6b-115">Сайтът може да използва твърде много ресурси и затова шаблонът на сайта надвишава ограничението от 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="82c6b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="82c6b-116">Има проблеми при показването на данни от списък, който използва справочна колона.</span><span class="sxs-lookup"><span data-stu-id="82c6b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="82c6b-117">За повече информация вижте [шаблон генерирани списък не показва данни от правилния списък](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)за търсене в SharePoint Online .</span><span class="sxs-lookup"><span data-stu-id="82c6b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="82c6b-118">За по-подробна информация относно често срещаните проблеми и решения, моля, проверете [Създаване и използване на шаблони на сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="82c6b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



