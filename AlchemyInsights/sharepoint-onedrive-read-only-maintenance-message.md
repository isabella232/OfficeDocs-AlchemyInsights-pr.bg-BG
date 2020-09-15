---
title: Съобщение "само за четене" за поддръжка при опит за използване на SharePoint или OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670821"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="97d83-102">Съобщение "само за четене" за поддръжка при опит за използване на SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="97d83-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="97d83-103">Потребителите могат да получат съобщение **за поддръжка само за четене** , когато се опитват да използват SharePoint или OneDrive за един от следните сценарии.</span><span class="sxs-lookup"><span data-stu-id="97d83-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="97d83-104">Планирана или активна дейност по поддръжката.</span><span class="sxs-lookup"><span data-stu-id="97d83-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="97d83-105">Проверете за тях, като навигирате до [центъра за съобщения](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="97d83-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="97d83-106">Инцидент с активна услуга с висок приоритет, който може да възникне.</span><span class="sxs-lookup"><span data-stu-id="97d83-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="97d83-107">Проверете за каквито и да е съвети/инциденти чрез навигация за [изправността на услугите](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="97d83-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="97d83-108">Малък сценарий за възстановяване на Auto-изцеление, който може да се случи поради всякакви неочаквани събития на сървърите, които може да траят по-малко от 30 минути.</span><span class="sxs-lookup"><span data-stu-id="97d83-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="97d83-109">Няма център за съобщения или публикации за здравна услуга за тези по-малки възстановени неща, но трябва да се върнете към нормалното си състояние много скоро.</span><span class="sxs-lookup"><span data-stu-id="97d83-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="97d83-110">В много малко случаи забелязахме, че един от трите сценария, изброени по-горе, е причината и услугата е възстановена, но кешът на браузъра за потребители не е изчистен.</span><span class="sxs-lookup"><span data-stu-id="97d83-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="97d83-111">Моля, опитайте да изчистите кеша на браузъра, преди да се придвижите до сайта.</span><span class="sxs-lookup"><span data-stu-id="97d83-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="97d83-112">В браузъра Microsoft Edge изберете **Настройки**и след това изберете **поверителност и защита**.</span><span class="sxs-lookup"><span data-stu-id="97d83-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="97d83-113">Под **Изчисти браузъра**изберете **Изберете какво да изчистите**.</span><span class="sxs-lookup"><span data-stu-id="97d83-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="97d83-114">Изберете **бисквитки и запазени данни за уеб сайта**и изберете **Изчисти**.</span><span class="sxs-lookup"><span data-stu-id="97d83-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="97d83-115">Тези стъпки може да се различават при използването на други браузъри, като Mozilla Firefox или Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="97d83-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="97d83-116">Друга възможност е да отворите вашия сайт на SharePoint или OneDrive в нов прозорец на InPrivate.</span><span class="sxs-lookup"><span data-stu-id="97d83-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>