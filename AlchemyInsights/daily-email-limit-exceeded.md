---
title: Превишена е дневната граница на имейла. Работният поток е спрян.
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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908693"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Превишен е дневният лимит на имейла. Работният поток е спрян.

Тази грешка може да бъде получена в следните ситуации:

- Имате работен поток в SharePoint Online, който използва sharePoint 2010 или SharePoint 2013 поток платформа тип.
- Работният поток е конфигуриран да изпраща имейл съобщение по избор на повече от 200 потребители наведнъж, повече от 10 000 получатели на ден или повече от 30 съобщения в минута.
- Когато стартирате работния поток, имейл съобщението не се изпраща и забележите следното поведение:
    - За работен поток с помощта на типа на платформата На SharePoint 2013 можете да преминете към страницата на състоянието на **работния поток.** На страницата състояние на работния поток **вътрешно то е** настроено на **"Стартирано"** и балонът с информация показва **не възможност за изпращане на получател**.

За да заобиколите този проблем, конфигурирайте работния поток да изпращате имейл съобщения без превишаване на ограниченията на [подателя на Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Например използвайте пауза в работния поток, изпратете имейл до група на Microsoft 365, група за разпространение или пощенска поддръжка на група за защита или изпращане на съобщението на по-малко от 200 получатели наведнъж.


За повече информация вижте следната [статия](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Сродни теми
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 