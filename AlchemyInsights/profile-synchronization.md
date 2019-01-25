---
title: Синхронизация на профили
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458652"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когато промените ми профил за синхронизиране на SharePoint приложението за потребителски профил?

SharePoint Online използва Active Directory внос заданието на таймера (AD внос) да импортиране на потребители и групи в приложението за потребителски профили. 
  
1. АД внос синхронизира промени от хранилището на SharePoint онлайн директория на приложението за потребителски профили. Тези промени се обработват на порции.
    
2. Заданието за таймер работи, докато промените бъдат синхронизирани.
    
> [!NOTE]
> Времето, необходимо за изпълнението на проекта зависи от броя на промените да обработи. Голям брой промени отнема повече време. Служба равнище споразумение (SLA) се посочва, че промяна на потребител в SharePoint онлайн директория ще бъдат отразени в приложението за потребителски профили в 24 часа. 
  
[Повече информация за синхронизиране на потребителски профили в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

