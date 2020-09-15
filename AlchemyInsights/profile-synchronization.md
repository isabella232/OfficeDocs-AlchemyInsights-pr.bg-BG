---
title: Синхронизиране на профили
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801758"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="fa30f-102">Кога промените в профила ми ще се синхронизират с приложението за потребителски профил на SharePoint?</span><span class="sxs-lookup"><span data-stu-id="fa30f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="fa30f-103">SharePoint online използва заданието за таймер за импортиране на Active Directory (импортиране на реклами), за да импортира потребители и групи в приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="fa30f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="fa30f-104">Импортирането на реклами синхронизира промените от магазина за справочен указател на SharePoint Online към приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="fa30f-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="fa30f-105">Тези промени се обработват в партиди.</span><span class="sxs-lookup"><span data-stu-id="fa30f-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="fa30f-106">Заданието за таймер се изпълнява, докато промените не бъдат синхронизирани.</span><span class="sxs-lookup"><span data-stu-id="fa30f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="fa30f-107">Времето, което е необходимо, за да се изпълни задачата, зависи от броя на промените в процеса.</span><span class="sxs-lookup"><span data-stu-id="fa30f-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="fa30f-108">Голяма част от промените отнема повече време.</span><span class="sxs-lookup"><span data-stu-id="fa30f-108">A large number of changes takes longer.</span></span> <span data-ttu-id="fa30f-109">Споразумението за ниво на обслужване (SLA) гласи, че промяната в указателя на SharePoint Online ще бъде отразена в приложението за потребителски профил за 24 часа.</span><span class="sxs-lookup"><span data-stu-id="fa30f-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="fa30f-110">Повече информация за синхронизирането на потребителски профили в SharePoint online</span><span class="sxs-lookup"><span data-stu-id="fa30f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

