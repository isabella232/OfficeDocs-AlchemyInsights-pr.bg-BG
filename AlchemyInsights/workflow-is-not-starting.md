---
title: Работният поток не се стартира
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738078"
---
# <a name="workflow-is-not-starting"></a>Работният поток не се стартира

- SharePoint 2010 и SharePoint 2013 работни потоци не се стартира.

    - Ако вашият работен поток не се стартира, може да има временен проблем с услугата, при който потребителите могат да изпитват периодични закъснения с напредъка на работния поток. Проверете [услугата Health табло](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.

    - Ако са изминали повече от 24 часа от първия път, когато сте видели този проблем, моля, впишете билет за поддръжка. В много случаи вече работим по решение. Моля, дайте ни поне 24 часа, за да завършим решение.

- Работни потоци на SharePoint 2010 забавени при стартиране.

    - Това се случва, ако работният поток се задейства в големи папки. (например, когато няколко елемента се добавят наведнъж).

    - Работните потоци не са предназначени за изпълнение в реално време, така че забавянето е поведението по дизайн.

   -  Ако работният поток е сложен разширен обект маркиране език (XMOL), компилация може да бъде бавен. Проверете [тази](https://support.microsoft.com//kb/3043697) статия.

    - Трябва да опростите работния поток или да го препроменяте с помощта на типа на платформата Microsoft SharePoint 2013 поток.

    - Ако хронологията на работния поток е пораснала голяма, може да искате да изчистите елементите или да създадете нов списък с хронология.

        Повече информация: [изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft Flow в SharePoint online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


