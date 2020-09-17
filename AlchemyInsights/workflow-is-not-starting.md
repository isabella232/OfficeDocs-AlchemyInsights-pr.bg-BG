---
title: Работният поток не се стартира
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794756"
---
# <a name="workflow-is-not-starting"></a>Работният поток не се стартира

- Работните потоци на SharePoint 2010 и SharePoint 2013 не се стартират.

    - Ако работният поток не се стартира, е възможно да има проблем с временен услуга, при който потребителите могат да се сблъскат с периодични закъснения с напредъка на работния поток. Проверете [таблото за изправност на услугите](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.

    - Ако са изминали повече от 24 часа, откакто за пръв път видяхте този проблем, можете да регистрирате билет за поддръжка. В много случаи вече работим върху решение. Моля, дайте ни най-малко 24 часа, за да завършите решение.

- Работните потоци на SharePoint 2010 се забавиха при стартиране.

    - Това се случва, ако работният поток се задейства в големи партиди. (например когато са добавени няколко елемента наведнъж).

    - Работните потоци не са предназначени да се изпълняват в реално време, така че закъснението е по-модел на поведение.

   -  Ако работният поток е сложен език за коректура на обекти (XMOL), съставянето може да бъде бавно. Проверете [тази](https://support.microsoft.com//kb/3043697) статия.

    - Трябва да опростите работния поток или да го препроектирате, като използвате типа платформа на работен поток на Microsoft SharePoint 2013.

    - Ако вашата хронология на работния поток е нараснал голям, може да поискате да изчистите елементите или да създадете нов списък с хронологии.

        Още информация: [изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродни теми
Искате да изпробвате Microsoft Flow в SharePoint online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


