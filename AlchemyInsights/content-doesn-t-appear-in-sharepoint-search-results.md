---
title: Съдържанието не се показва в SharePoint от търсенето
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081599"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Съдържанието не се показва в SharePoint от търсенето

Следвайте тези стъпки за отстраняване на неизправности, когато очакваното съдържание не се показва в резултатите от търсенето:
  
1. Проверете дали **сайтът, съдържащ** очакваното съдържание, е настроен така, че съдържанието да се показва в резултатите от търсенето. Следвайте стъпките в [Показване на съдържание в сайт в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Проверете дали списъкът **или библиотеката,** **които съдържат** очакваното съдържание, са настроени да позволяват съдържанието да се показва в резултатите от търсенето. Следвайте стъпките в [Показване на съдържание от списъци или библиотеки в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Уверете се, че оформлението на страницата, документа или страницата по избор е публикувано като **основна версия.** Следвайте стъпка 3 [в "Търсене" не връща всички резултати в SharePoint онлайн.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Уверете се, че потребителят **има разрешения за** преглед на съдържанието. Следвайте стъпките в [Разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ако схемата за търсене е променена чрез добавяне на ново управлявано свойство, чрез редактиране на управлявано свойство или чрез премахване на управлявано свойство, тогава ще се изисква искане за обхождане и повторно индексиране. **Преоценяване** на съдържанието, като следвате стъпките в Ръчно искане за обхождане и повторно индексиране на [сайт, библиотека или списък](https://docs.microsoft.com/sharepoint/crawl-site-content). Това може да отнеме известно време, изчакайте 24 часа, преди да проверите резултатите отново.

За повече информация вижте Разрешаване [на съдържание в сайт за търсене.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
