---
title: Лимитът на ежедневните имейли е превишен. Работният поток е спрян.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053106"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Ограничение на дневния имейл лимит. Работният поток е спрян.

Тази грешка може да бъде получена в следните сценарии:

- Имате работен поток в SharePoint Online, използващ SharePoint 2010 или SharePoint 2013 работен поток платформа тип.
- Работният поток е конфигуриран да изпраща потребителски имейл съобщение до повече от 200 потребители наведнъж, повече от 10 000 получатели на ден, или повече от 30 съобщения в минута.
- Когато стартирате работния поток, имейл съобщението не се изпраща и забележите следното поведение:
    - За работен поток с помощта на SharePoint 2013 платформа тип преминете към страницата на **състоянието на работния поток** . На страницата състояние на работния поток **вътрешно състояние** е настроен да **стартира**и информация балон показва **не може да изпрати на получател**.

За да заобиколите този проблем, конфигурирайте вашия работен поток за изпращане на имейл съобщения, без да надвишава [границите на Exchange Online подател](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например използвайте пауза в работния поток, изпращане на имейл до група на Office 365, група за разпространение или електронна поща разрешено група за защита, или изпращане на съобщението до по-малко от 200 получатели наведнъж.


За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Сродни теми
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 