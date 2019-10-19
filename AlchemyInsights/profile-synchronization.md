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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Кога Моят профил променя синхронизирането на приложението за потребителски профили на SharePoint?

SharePoint online използва Active Directory импортиране таймер задание (AD импортиране) за импортиране на потребители и групи в приложението за потребителски профили. 
  
1. Импортиране на AD синхронизира промени от SharePoint online директория хранилище на приложението за потребителски профили. Тези промени се обработват в партиди.
    
2. Заданието на таймера се изпълнява, докато промените не се синхронизират.
    
> [!NOTE]
> Времето, необходимо за изпълнение на заданието, зависи от броя на промените, които трябва да се обработят. Голям брой промени отнема повече време. Споразумението за ниво на обслужване (SLA) гласи, че промяна на потребител в SharePoint online директория ще се отрази в приложението за потребителски профили в 24 часа. 
  
[Повече информация за синхронизиране на потребителски профили в SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

