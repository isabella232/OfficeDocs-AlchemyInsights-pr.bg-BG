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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923633"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Кога се променя синхронизирането на моя профил с SharePoint приложение за потребителски профил?

SharePoint Онлайн използва заданието на таймера за импортиране на Active Directory (импортиране на AD), за да импортира потребители и групи в приложението за потребителски профил. 
  
1. Импортирането на AD синхронизира промените от SharePoint онлайн справочника в приложението за потребителски профили. Тези промени се обработват в партиди.
    
2. Заданието на таймера се изпълнява, докато промените не се синхронизират.
    
> [!NOTE]
> Времето, необходимо за изпълнение на задачата, зависи от броя на промените, които трябва да обработите. Голям брой промени отнема повече време. Споразумението за ниво на услугата (SLA) гласи, че промяната на потребител в онлайн справочната SharePoint ще бъде отразена в приложението за потребителски профил след 24 часа. 
  
[Повече информация за синхронизирането на потребителски профили в SharePoint Онлайн](https://go.microsoft.com/fwlink/?linkid=875671)
  

