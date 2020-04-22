---
title: Съдържанието не се показва в резултатите от търсенето на SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705650"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Съдържанието не се показва в резултатите от търсенето на SharePoint

Следвайте тези стъпки за отстраняване на неизправности, когато очакваното съдържание не се показва в резултатите от търсенето:
  
1. Проверете дали **сайтът,** който съдържа очакваното съдържание, е настроен да позволява съдържанието да се показва в резултатите от търсенето. Следвайте стъпките в [Показване на съдържание на сайт в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Проверете дали **списъкът** или **библиотеката,** които съдържат очакваното съдържание, е настроен да разрешава показването на съдържание в резултатите от търсенето. Следвайте стъпките в [Показване на съдържание от списъци или библиотеки в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Проверете дали оформлението на страницата, документа или персонализираното оформление на страницата е публикувано като **основна версия.** Следвайте стъпка 3 в [търсене не връща всички резултати в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Проверете дали потребителят има **разрешения** да преглежда съдържанието. Следвайте стъпките в [Разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ако схемата на търсене е променена чрез добавяне на ново контролирано свойство, чрез редактиране на контролирано свойство или чрез премахване на контролирано свойство, тогава ще се изисква обхождане и повторно индексиране. **Индексирайте повторно** съдържанието, като следвате стъпките в [Ръчно поискате обхождане и повторно индексиране на сайт, библиотека или списък](https://docs.microsoft.com/sharepoint/crawl-site-content). Това може да отнеме известно време, изчакайте 24 часа, преди да проверите резултатите отново.

За повече информация вижте [Разрешаване на съдържание на сайт, за да може да се търси](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
