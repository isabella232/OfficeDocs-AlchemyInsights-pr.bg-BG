---
title: Проблеми с производителността-SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068380"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive бавни, недостъпни или недостъпни за няколко потребители

SharePoint или OneDrive може да е бавен, недостъпен или недостъпен, или може да показва недостъпна услуга или 503 грешки по няколко причини:
  
- Ако сайтът ви в SharePoint или OneDrive е бавен или отложен за няколко потребители, може да има временен проблем с услугата, при който потребителите изпитват периодични закъснения или навигационни грешки при достъп до сайтове на SharePoint или съдържание в OneDrive. Проверете [таблото за изправността на услугата](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.
  
- Потребителите могат да получат *503 сървър е зает* грешка при опит за навигиране до сайтове на SharePoint или OneDrive. Тази грешка може да бъде причинена от ограничаване на услугата на SharePoint. SharePoint online използва ограничаване за поддържане на оптимална производителност и надеждност на услугата на SharePoint online. Ограничаването на броя на действията на потребителя или едновременни повиквания (със скрипт или код) за предотвратяване на прекомерната употреба на ресурси. За повече информация за ограничаване Вижте, [Избягвайте да ограничил или блокирани в SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ако имате ниска производителност с **класически** или **модерен** сайт на SharePoint или страница, използвайте инструмента за [диагностика на страницата](https://aka.ms/perftool) , за да анализирате страниците.
  
- Ако все още имате общи ниска производителност, прегледайте ресурсите в долната част на тази статия: [Въведение в настройката на производителността за SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  