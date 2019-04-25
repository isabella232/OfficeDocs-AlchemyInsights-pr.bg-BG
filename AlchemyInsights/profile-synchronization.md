---
title: Синхронизация на профили
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371973"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="50246-102">Когато промените ми профил за синхронизиране на SharePoint приложението за потребителски профил?</span><span class="sxs-lookup"><span data-stu-id="50246-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="50246-103">SharePoint Online използва Active Directory внос заданието на таймера (AD внос) да импортиране на потребители и групи в приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="50246-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="50246-104">АД внос синхронизира промени от хранилището на SharePoint онлайн директория на приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="50246-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="50246-105">Тези промени се обработват на порции.</span><span class="sxs-lookup"><span data-stu-id="50246-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="50246-106">Заданието за таймер работи, докато промените бъдат синхронизирани.</span><span class="sxs-lookup"><span data-stu-id="50246-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="50246-107">Времето, необходимо за изпълнението на проекта зависи от броя на промените да обработи.</span><span class="sxs-lookup"><span data-stu-id="50246-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="50246-108">Голям брой промени отнема повече време.</span><span class="sxs-lookup"><span data-stu-id="50246-108">A large number of changes takes longer.</span></span> <span data-ttu-id="50246-109">Служба равнище споразумение (SLA) се посочва, че промяна на потребител в SharePoint онлайн директория ще бъдат отразени в приложението за потребителски профили в 24 часа.</span><span class="sxs-lookup"><span data-stu-id="50246-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="50246-110">Повече информация за синхронизиране на потребителски профили в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="50246-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

