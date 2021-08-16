---
title: MC210173 – SharePoint Designer – прекратяване на функцията за нов формуляр по избор
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077641"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – SharePoint Designer – прекратяване на функцията за нов формуляр по избор

Установихме проблем, засягащ функционалността на SharePoint Designer за [създаване на персонализирани формуляри](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) в SharePoint Online. След внимателен преглед установихме, че няма известна корекция за този проблем и избрахме да забраним функцията за създаване на персонализиран формуляр, което влиза в сила в 3:00 преди обяд UTC в събота, 25 април 2020 г. Тази промяна не оказва влияние върху възможността за редактиране на предварително създадени формуляри, или върху други съществуващи функции в SharePoint Online Designer.

След като е направена тази промяна, възможно е потребителите да са получили грешката: "Не може да се запишат промените в списъка в сървъра" при създаване на нови формуляри.

Потребителите, които преди това са използвали SharePoint Designer за създаване на персонализирани формуляри, могат вместо това да използват [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) за тази цел.

PowerApps е лесен и мощен инструмент, който позволява на потребителите да работят в модерната среда на SharePoint Online, за да създават и редактират персонализирани формуляри за списъци в SharePoint и библиотеки с документи директно от прозореца на браузъра. PowerApps не изисква традиционните знания за кодиране или някакви допълнителни изтегляния на приложения, например InfoPath.

**Бележка**: Потребителите на класическата среда в SharePoint Online ще трябва временно да преминат към работа в модерна среда, за да имат достъп и да използват PowerApps; въпреки че до всички персонализирани формуляри, създадени в PowerApps, потребителите на класическата среда в SharePoint Online имат достъп.
