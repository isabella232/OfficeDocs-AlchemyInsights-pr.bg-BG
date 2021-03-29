---
title: Работният поток не започва
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403732"
---
# <a name="workflow-is-not-starting"></a>Работният поток не започва

- Работните потоци на SharePoint 2010 и SharePoint 2013 не се стартират.

    - Ако вашият работен поток не се стартира, може да има временен проблем с услугата, при който потребителите може да изпитват неспоменато забавяне с напредъка на работния поток. Проверете [таблото за изтезания на](https://admin.microsoft.com/AdminPortal/Home/servicehealth) услугите, за да видите дали вашата организация е засегнати.

    - Ако са минали повече от 24 часа, откакто за първи път сте видели този проблем, влезте в билет за поддръжка. В много случаи вече работим по решение. Дайте ни поне 24 часа, за да завършим решение.

- Работните потоци на SharePoint 2010 се забавят при стартиране.

    - Това се случва, ако работният поток се активира в големи партиди. (например когато се добавят няколко елемента наведнъж).

    - Работните потоци не са предназначени да се изпълняват в реално време, така че забавянето е поведението при проектиране.

   -  Ако работният поток е сложен език за маркиране на разширяеми обекти (XMOL), компилацията може да бъде бавна. Проверете [тази](https://support.microsoft.com//kb/3043697) статия.

    - Трябва да опростите работния поток или да го пренавивате с помощта на типа платформа за работни потоци на Microsoft SharePoint 2013.

    - Ако хронологията на работния поток е нараснала голяма, може да искате да прочистите елементите или да създадете нов списък с хронология.

        Повече информация: [Изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродни теми
Искате да изпробвате Microsoft Flow в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
