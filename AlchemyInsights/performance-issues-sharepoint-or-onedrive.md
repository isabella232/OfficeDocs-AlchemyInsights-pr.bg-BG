---
title: Проблеми с производителността – SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771890"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive – бавен, недостъпен или недостъпен за множество потребители

SharePoint или OneDrive може да е бавен, недостъпен или недостъпен или може да показва услугата недостъпни или 503 грешки по няколко причини:
  
- Ако вашият сайт на SharePoint или OneDrive е бавен или забавен за много потребители, е възможно да има проблем с временните услуги, в който потребителите да получават периодични закъснения или грешки при навигация при достъп до сайтове на SharePoint или съдържание на OneDrive. Проверете [таблото за изправност на услугите](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.
  
- Потребителят може да получи съобщение за грешка, че *сървърът на 503 е зает* при опит за навигиране до сайтове на SharePoint или OneDrive. Тази грешка може да се дължи на ограничаване в рамките на услугата на SharePoint. SharePoint Online използва регулиране, за да поддържа оптимална производителност и надеждност на услугата SharePoint Online. Регулирането ограничава броя на действията на потребителите или едновременните повиквания (по скрипт или код), за да се предотврати прекомерната употреба на ресурси. За повече информация относно ограничаването на скоростта вижте [избягване на ограничаването или блокирането в SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ако имате ниска производителност с **класически** или **модерен** сайт на SharePoint или страница, използвайте инструмента за [диагностика](https://aka.ms/perftool) на страници, за да анализирате страниците.
  
- Ако все още имате общи бавни резултати, прегледайте ресурсите в долната част на тази статия: [Въведение в настройката на производителността за SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  