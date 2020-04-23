---
title: Синхронизация на профили
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768102"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Кога промени те се синхронизират с приложението за потребителски профили на SharePoint?

SharePoint Online използва active Directory импортиране таймер задание (AD импортиране) за импортиране на потребители и групи в приложението за потребителски профили. 
  
1. Импортиране на РЕКЛАМА синхронизира промени от хранилището на SharePoint Online директория на приложението за потребителски профили. Тези промени се обработват в пакети.
    
2. Заданието на таймера се изпълнява, докато промените се синхронизират.
    
> [!NOTE]
> Времето, необходимо за изпълнение на проекта, зависи от броя на промените в процеса. Голям брой промени отнемат повече време. Споразумението за ниво на услугата (SLA) гласи, че промяна на потребител в SharePoint Online Directory ще се отразят в приложението за потребителски профили в 24 часа. 
  
[Повече информация за синхронизиране на потребителски профили в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

