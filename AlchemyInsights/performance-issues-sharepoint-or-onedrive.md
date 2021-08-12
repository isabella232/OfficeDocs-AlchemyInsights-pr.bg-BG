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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911831"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive бавни, недостъпни или недостъпни за няколко потребители

SharePoint или OneDrive може да са бавни, недостъпни или недостъпни или да показват услугата недостъпна или 503 грешки поради няколко причини:
  
- Ако вашият сайт SharePoint или OneDrive е бавен или забавен за няколко потребители, може да има временен проблем с услугата, при който потребителите изпитват периодично забавяне или грешки в навигацията при достъп до SharePoint сайтове или OneDrive съдържание. Проверете [таблото за изтезания на](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) услугите, за да видите дали вашата организация е засегнати.
  
- Потребителите може да получат *грешка 503 сървър,* когато се опитват да навигират до SharePoint или OneDrive сайтове. Тази грешка може да се дължи на ограничаването в SharePoint услугата. SharePoint Online използва регулиране, за да поддържа оптимална производителност и надеждност на услугата SharePoint Online. Регулирането ограничава броя на действията на потребителите или едновременните повиквания (по скрипт или код), за да се предотврати прекомерната употреба на ресурси. За повече информация относно ограничаването вижте Избягване на ограничаване или блокиране [в SharePoint онлайн.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Ако имате бавна производителност с класически **или** **модерен** SharePoint сайт или страница, използвайте инструмента за диагностика на [страниците, за](https://aka.ms/perftool) да анализирате страниците.
  
- Ако все още имате обща бавна производителност, прегледайте ресурсите в долната част на тази статия: Въведение в [настройването на производителността за SharePoint Онлайн](https://go.microsoft.com/fwlink/?linkid=2024334)
  