---
title: Синхронизиране на профили
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554322"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="4282f-102">Кога Моят профил променя синхронизирането на приложението за потребителски профили на SharePoint?</span><span class="sxs-lookup"><span data-stu-id="4282f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="4282f-103">SharePoint online използва Active Directory импортиране таймер задание (AD импортиране) за импортиране на потребители и групи в приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="4282f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="4282f-104">Импортиране на AD синхронизира промени от SharePoint online директория хранилище на приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="4282f-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="4282f-105">Тези промени се обработват в партиди.</span><span class="sxs-lookup"><span data-stu-id="4282f-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="4282f-106">Заданието на таймера се изпълнява, докато промените не се синхронизират.</span><span class="sxs-lookup"><span data-stu-id="4282f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="4282f-107">Времето, необходимо за изпълнение на заданието, зависи от броя на промените, които трябва да се обработят.</span><span class="sxs-lookup"><span data-stu-id="4282f-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="4282f-108">Голям брой промени отнема повече време.</span><span class="sxs-lookup"><span data-stu-id="4282f-108">A large number of changes takes longer.</span></span> <span data-ttu-id="4282f-109">Споразумението за ниво на обслужване (SLA) гласи, че промяна на потребител в SharePoint online директория ще се отрази в приложението за потребителски профили в 24 часа.</span><span class="sxs-lookup"><span data-stu-id="4282f-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="4282f-110">Повече информация за синхронизиране на потребителски профили в SharePoint online</span><span class="sxs-lookup"><span data-stu-id="4282f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

