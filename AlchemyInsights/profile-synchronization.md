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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554322"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7f721-102">Когато промените ми профил за синхронизиране на SharePoint приложението за потребителски профил?</span><span class="sxs-lookup"><span data-stu-id="7f721-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7f721-103">SharePoint Online използва Active Directory внос заданието на таймера (AD внос) да импортиране на потребители и групи в приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="7f721-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7f721-104">АД внос синхронизира промени от хранилището на SharePoint онлайн директория на приложението за потребителски профили.</span><span class="sxs-lookup"><span data-stu-id="7f721-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="7f721-105">Тези промени се обработват на порции.</span><span class="sxs-lookup"><span data-stu-id="7f721-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7f721-106">Заданието за таймер работи, докато промените бъдат синхронизирани.</span><span class="sxs-lookup"><span data-stu-id="7f721-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7f721-107">Времето, необходимо за изпълнението на проекта зависи от броя на промените да обработи.</span><span class="sxs-lookup"><span data-stu-id="7f721-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="7f721-108">Голям брой промени отнема повече време.</span><span class="sxs-lookup"><span data-stu-id="7f721-108">A large number of changes takes longer.</span></span> <span data-ttu-id="7f721-109">Служба равнище споразумение (SLA) се посочва, че промяна на потребител в SharePoint онлайн директория ще бъдат отразени в приложението за потребителски профили в 24 часа.</span><span class="sxs-lookup"><span data-stu-id="7f721-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7f721-110">Повече информация за синхронизиране на потребителски профили в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7f721-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

