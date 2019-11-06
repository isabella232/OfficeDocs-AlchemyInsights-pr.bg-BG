---
title: 2609-задържане-или-откриване на
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994044"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="e3bda-102">Не можете да изтриете елементи в SharePoint Online или OneDrive за бизнес</span><span class="sxs-lookup"><span data-stu-id="e3bda-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="e3bda-103">Вие или вашите потребители може да не можете да изтриете елементи в SharePoint Online или OneDrive за бизнес, защото правила за задържане, етикет за задържане или откриване на електронни съобщения се прилага към SharePoint на сайта на OneDrive или конкретен елемент.</span><span class="sxs-lookup"><span data-stu-id="e3bda-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="e3bda-104">Това включва невъзможност за изтриване на документ, версия на документ, папка, Библиотека с документи, списък, приложение, сайт или колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="e3bda-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="e3bda-105">Ето няколко примера за съобщенията за грешки, които може да получите, ако се опитате да изтриете елемент, който се запазва:</span><span class="sxs-lookup"><span data-stu-id="e3bda-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="e3bda-106">"Този сайт не може да бъде изтрит, защото е включен в задържане или политика на задържане"</span><span class="sxs-lookup"><span data-stu-id="e3bda-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e3bda-107">"Този сайт има правила за съответствие, зададени за блокиране на изтриването"</span><span class="sxs-lookup"><span data-stu-id="e3bda-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="e3bda-108">"Правилата за съответствие в момента блокират този сайт изтриване"</span><span class="sxs-lookup"><span data-stu-id="e3bda-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="e3bda-109">"Тази колекция от сайтове не може да бъде изтрита, тъй като съдържа сайтове, които са включени в задържане или политика на задържане"</span><span class="sxs-lookup"><span data-stu-id="e3bda-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e3bda-110">"Трябва да изтриете всички елементи в тази папка, преди да изтриете папката"</span><span class="sxs-lookup"><span data-stu-id="e3bda-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="e3bda-111">"Версиите на този елемент не могат да бъдат изтрити, защото са на задържане или правила за запазване"</span><span class="sxs-lookup"><span data-stu-id="e3bda-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="e3bda-112">"Елементът не може да бъде изтрит по време на задържане"</span><span class="sxs-lookup"><span data-stu-id="e3bda-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="e3bda-113">"Етикетът, който се прилага към този елемент не позволява да се редактира или изтрива"</span><span class="sxs-lookup"><span data-stu-id="e3bda-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="e3bda-114">"Списъкът не може да бъде изтрит по време на задържане или правила за задържане"</span><span class="sxs-lookup"><span data-stu-id="e3bda-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="e3bda-115">"Списъкът не може да бъде изтрит, ако е блокиран или ако правилата за задържане се прилагат към него"</span><span class="sxs-lookup"><span data-stu-id="e3bda-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="e3bda-116">За да изтриете елементи в един от тези сценарии, правила за задържане, етикет за задържане или откриване на откриването трябва да бъдат премахнати (или сайт трябва да бъде изключен от правила за задържане).</span><span class="sxs-lookup"><span data-stu-id="e3bda-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="e3bda-117">Трябва или да забраните, или да изключите съответното задържане, което причинява този проблем.</span><span class="sxs-lookup"><span data-stu-id="e3bda-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e3bda-118">След премахване на правила или задържане се премахва, може да отнеме до 24 часа, за да влязат в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="e3bda-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="e3bda-119">За информация относно различните функции за запазване и задържане, които могат да се приложат към сайтовете на SharePoint и профилите в OneDrive, вижте една от следните теми.</span><span class="sxs-lookup"><span data-stu-id="e3bda-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="e3bda-120">Преглед на правилата за задържане</span><span class="sxs-lookup"><span data-stu-id="e3bda-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="e3bda-121">Преглед на етикетите за задържане</span><span class="sxs-lookup"><span data-stu-id="e3bda-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="e3bda-122">Управление на задържания в Разширено откриване на</span><span class="sxs-lookup"><span data-stu-id="e3bda-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="e3bda-123">Откриването на откриване на</span><span class="sxs-lookup"><span data-stu-id="e3bda-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="e3bda-124">Правила за затваряне и изтриване на наследени сайтове</span><span class="sxs-lookup"><span data-stu-id="e3bda-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
