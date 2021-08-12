---
title: Ограничението за дневен имейл е надвишено. Работният поток е временно преустановен.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914640"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Ограничението за дневен имейл е превишено. Работният поток е временно преустановен.

Тази грешка може да бъде получена в следните сценарии:

- Имате работен поток в SharePoint Онлайн, който използва типа платформа SharePoint 2010 или SharePoint 2013.
- Работният поток е конфигуриран да изпраща имейл съобщение по избор до повече от 200 потребители едновременно, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.
- Когато изпълните работния поток, имейл съобщението не се изпраща и забележите следното поведение:
    - За работен поток, който използва SharePoint 2013 тип платформа, ще отидете на страницата Състояние **на работния** поток. На страницата Състояние на работния поток **вътрешното състояние** е зададено на **"Стартирано",** а балонът с информация **показва Не може да се изпрати до получател**.

За да заобиколите този проблем, конфигурирайте работния поток да изпраща имейл съобщения, без да [надвишавате Exchange Online на подателя.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Например използвайте пауза в работния поток, изпратете имейла до група на Microsoft 365, група за разпространение или група за защита с разрешена поща или изпратете съобщението на по-малко от 200 получатели едновременно.


За повече информация вижте следната [статия.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Сродни теми
- [Създаване на Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 