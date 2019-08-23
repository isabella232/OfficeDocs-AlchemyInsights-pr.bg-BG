---
title: Не стартиране на работен поток
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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557958"
---
# <a name="workflow-is-not-starting"></a>Не стартиране на работен поток

- SharePoint 2010 и SharePoint 2013 работни потоци не се започва.

    - Ако не се стартира работния поток, може да има проблем при временна услуга където потребителите могат да изпитат прекъсвания отлагам с поток прогрес. Проверете [Услуги здравето таблото](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) за да видите дали вашата организация е ударена.

    - Ако повече от 24 часа са изминали от вас за първи път видях този проблем, моля влезте билет подкрепа. В много случаи ние вече работим върху решение. Моля, дайте ни най-малко 24 часа да завършите решение.

- SharePoint 2010 работни потоци, които бавят Старт.

    - Това се случва, ако работният поток се задейства в големи партиди. (например, когато няколко позиции се добавят наведнъж).

    - Работните потоци не са проектирани да работят в реално време, така че закъснението е по проект поведение.

   -  Ако работният поток е сложна разтегателен обект Markup език (XMOL), компилация може да бъде бавно. Проверете [тази](https://support.microsoft.com/en-us/kb/3043697) статия.

    - Трябва да опрости работния поток или го използва Microsoft SharePoint 2013 поток платформа тип редизайн.

    - Ако хронологията на работния поток е нараснал големи, може да искате да прочисти елементи или да създадете нов списък с хронологии.

        Повече информация: [Изтриване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft поток в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


