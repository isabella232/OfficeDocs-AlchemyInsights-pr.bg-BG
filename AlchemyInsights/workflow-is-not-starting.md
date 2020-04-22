---
title: Работният поток не започва
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766086"
---
# <a name="workflow-is-not-starting"></a>Работният поток не започва

- SharePoint 2010 и SharePoint 2013 работни потоци не се стартира.

    - Ако вашият работен поток не се стартира, може да има временен проблем, когато потребителите могат да възникнат временни забавяния с напредъка на работния поток. Проверете [таблото за изправност](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) на услугата, за да видите дали вашата организация е повлияна.

    - Ако са изминали повече от 24 часа, откакто за първи път видяхте този проблем, моля, регистрирайте билет за поддръжка. В много случаи вече работим по решение. Моля, дайте ни поне 24 часа, за да завършите решение.

- SharePoint 2010 работни потоци забавяне при стартиране.

    - Това се случва, ако поток се задейства в големи папки. (например, когато се добавят няколко елемента едновременно).

    - Работните потоци не са проектирани да работят в реално време, така че забавянето е по-проектно поведение.

   -  Ако работният поток е сложен разширим обект markup Language (XMOL), компилация може да бъде бавно. Проверете [тази](https://support.microsoft.com//kb/3043697) статия.

    - Трябва да опрости работния поток или да го редизайн с помощта на microsoft SharePoint 2013 поток платформа тип.

    - Ако вашата хронология на работния поток е нараснала, може да искате да изчистите елементите или да създадете нов списък с хронология.

        Повече информация: [Прочистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft Flow в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


