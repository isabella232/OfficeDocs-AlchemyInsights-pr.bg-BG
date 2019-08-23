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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Когато промените ми профил за синхронизиране на SharePoint приложението за потребителски профил?

SharePoint Online използва Active Directory внос заданието на таймера (AD внос) да импортиране на потребители и групи в приложението за потребителски профили. 
  
1. АД внос синхронизира промени от хранилището на SharePoint онлайн директория на приложението за потребителски профили. Тези промени се обработват на порции.
    
2. Заданието за таймер работи, докато промените бъдат синхронизирани.
    
> [!NOTE]
> Времето, необходимо за изпълнението на проекта зависи от броя на промените да обработи. Голям брой промени отнема повече време. Служба равнище споразумение (SLA) се посочва, че промяна на потребител в SharePoint онлайн директория ще бъдат отразени в приложението за потребителски профили в 24 часа. 
  
[Повече информация за синхронизиране на потребителски профили в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

