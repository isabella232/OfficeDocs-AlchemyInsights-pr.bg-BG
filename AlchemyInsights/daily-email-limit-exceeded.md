---
title: Надвишено е дневното ограничение за имейл. Работният поток е прекъснат.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580322"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Лимитът за дневен имейл е надвишен. Работният поток е прекъснат.

Тази грешка може да бъде получена в следните ситуации:

- Имате работен поток в SharePoint Online, който използва SharePoint 2010 или SharePoint 2013 поток тип.
- Работният поток е конфигуриран да изпраща имейл съобщение по избор на повече от 200 потребители наведнъж, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.
- Когато стартирате работния поток, имейл съобщението не се изпраща и забележите следното поведение:
    - За работен поток с помощта на типа платформа SharePoint 2013, преминете към страницата за състояние на **работния поток.** На страницата Състояние на работния поток **вътрешното състояние** е зададено на **Стартиран**, а информационният балон показва **Не може да бъде изпратено до получател**.

За да заобиколите този проблем, конфигурирайте работния поток да изпращате имейл съобщения без превишаване на ограниченията на [подателя на Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например използвайте пауза в работния поток, изпратете имейл до група на Microsoft 365, група за разпространение или група за защита с разрешени имейли или изпратете съобщението на по-малко от 200 получатели едновременно.


За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Сродни теми
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 