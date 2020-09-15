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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Кога промените в профила ми ще се синхронизират с приложението за потребителски профил на SharePoint?

SharePoint online използва заданието за таймер за импортиране на Active Directory (импортиране на реклами), за да импортира потребители и групи в приложението за потребителски профили. 
  
1. Импортирането на реклами синхронизира промените от магазина за справочен указател на SharePoint Online към приложението за потребителски профили. Тези промени се обработват в партиди.
    
2. Заданието за таймер се изпълнява, докато промените не бъдат синхронизирани.
    
> [!NOTE]
> Времето, което е необходимо, за да се изпълни задачата, зависи от броя на промените в процеса. Голяма част от промените отнема повече време. Споразумението за ниво на обслужване (SLA) гласи, че промяната в указателя на SharePoint Online ще бъде отразена в приложението за потребителски профил за 24 часа. 
  
[Повече информация за синхронизирането на потребителски профили в SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

