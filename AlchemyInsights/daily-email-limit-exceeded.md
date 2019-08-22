---
title: Ежедневно имейл граница превишавам. Работният поток е спряно.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514430"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Всекидневен email граница превишавам. Работният поток е спряно.

Тази грешка може да бъдат получени в следните сценарии:

- Имате работен поток в SharePoint Online, която използва SharePoint 2010 или SharePoint 2013 поток платформа тип.
- Работният поток е конфигуриран за изпращане на персонализирани имейл съобщение до повече от 200 потребители в даден момент, повече от 10000 получатели на ден или повече от 30 съобщения в минута.
- Когато стартирате работния поток, имейл съобщението не е изпратено, и забележите следното поведение:
    - За работен поток, като използвате SharePoint 2013 платформа тип преминете към страницата на **Състоянието на работния поток** . В страницата състояние на работния поток **Вътрешно състояние** е настроено да **започнем**и балона с информация показва **не може да изпрати на получател**.

За да заобиколите този проблем, конфигурирайте вашия работен поток да изпрати имейл съобщения без превишаване на [Exchange Online подателя граници](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например използвайте пауза в работния поток, изпращане на имейл до Office 365 група, група за разпространение или група за защита на поща разрешени или изпращане на съобщение до по-малко от 200 получатели в даден момент.


За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Сродни теми
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 