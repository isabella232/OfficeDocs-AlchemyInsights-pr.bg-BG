---
title: Ограничението за дневен имейл е надвишено. Работният поток се отменя.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731552"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Ограничението за дневен имейл е надвишено. Работният поток се отменя.

Тази грешка може да бъде получена в следните сценарии:

- Имате работен поток в SharePoint Online, който използва типа на платформата за работен поток на SharePoint 2010 или SharePoint 2013.
- Работният поток е конфигуриран да изпраща имейл съобщение по избор до повече от потребители на 200 едновременно, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.
- Когато стартирате работния поток, имейл съобщението не се изпраща и забелязвате следното поведение:
    - За работен поток, използващ типа платформа на SharePoint 2013, трябва да отидете на страницата " **състояние на работния поток** ". В страницата "състояние на работния поток" **вътрешното състояние** е зададено на " **стартиран**" и балонът с информация **не може да се изпрати до получателя**.

За да заобиколите този проблем, конфигурирайте своя работен поток, за да изпращате имейл съобщения, без да надвишавате [ограничението за подателя на Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например използвайте пауза в работния поток, изпратете имейла до група на Microsoft 365, група за разпространение или група за защита с активиран имейл или изпратете съобщението до по-малко от 200 получатели едновременно.


За повече информация вижте [статията](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)по-долу.

## <a name="related-topics"></a>Сродни теми
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 