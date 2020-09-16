---
title: Създаване на сайт в SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732201"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="811f9-102">Създаване на сайтове на SharePoint с помощта на шаблони</span><span class="sxs-lookup"><span data-stu-id="811f9-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="811f9-103">Възможността за записване на сайт като шаблон не се поддържа със съвременните комуникационни или екипни сайтове.</span><span class="sxs-lookup"><span data-stu-id="811f9-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="811f9-104">За повече информация относно използването на шаблони вижте [записване, изтегляне и качване на сайт на SharePoint като шаблон](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="811f9-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="811f9-105">Ето някои често срещани проблеми/решения относно записването на сайт или списък като шаблон в SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="811f9-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="811f9-106">**Бутонът "записване на шаблон на сайт/списък" не е наличен или липсва**</span><span class="sxs-lookup"><span data-stu-id="811f9-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="811f9-107">Администраторите ще трябва да разрешат скриптовете по избор да разрешат функциите на шаблона.</span><span class="sxs-lookup"><span data-stu-id="811f9-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="811f9-108">За подробни стъпки, примери и съображения вижте</span><span class="sxs-lookup"><span data-stu-id="811f9-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="811f9-109">Разрешаване или забраняване на скрипт по избор</span><span class="sxs-lookup"><span data-stu-id="811f9-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="811f9-110">Командата Запиши сайта като шаблон не се поддържа и може да доведе до проблеми в сайтовете, които използват инфраструктурата за публикуване на SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="811f9-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="811f9-111">**Шаблонът за сайт не може да бъде създаден или не работи правилно**</span><span class="sxs-lookup"><span data-stu-id="811f9-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="811f9-112">Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и няма да се активира.</span><span class="sxs-lookup"><span data-stu-id="811f9-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="811f9-113">Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона за сайт, за да създадете сайт.</span><span class="sxs-lookup"><span data-stu-id="811f9-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="811f9-114">Проверете дали някакви списъци или библиотеки не надвишават [прага на списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) на елементите на 5000, тъй като това може да блокира създаването на шаблон за сайт.</span><span class="sxs-lookup"><span data-stu-id="811f9-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="811f9-115">Сайтът може да използва твърде много ресурси и следователно шаблонът на сайта надвишава ограничението за 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="811f9-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="811f9-116">Има проблеми при показване на данни от списък, който използва колоната за справки.</span><span class="sxs-lookup"><span data-stu-id="811f9-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="811f9-117">За повече информация вижте [списък, генериран от шаблон, не показва данни от правилния справочен списък в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="811f9-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="811f9-118">За по-подробна информация относно често срещаните проблеми и решения вижте [Създаване и използване на шаблони за сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="811f9-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



