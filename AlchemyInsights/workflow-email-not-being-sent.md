---
title: Имейл процес не се изпраща
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
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766122"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Имейл на работен поток не се изпраща за списък или библиотека на SharePoint

1. Имейл от работни потоци не се изпраща до всички потребители или само конкретни потребители, или виждате грешка **Имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.

    Проверете дали потребителят съществува в групата **разрешения за всички хора** (списък с информация за потребители) за тази колекция от сайтове.  Примерен директен<tenant>URL<sitename>адрес: https:// .sharepoint.com/sites/ /_layouts/15/people.aspx? ИД на група за членство=0

    - Ако потребителят не съществува, уверете се, че потребителят е влязъл в страницата. 
    - Ако е външен потребител, уверете се, че поканата му е приета.
    - Ако потребителят съществува в групата разрешения, уверете се, че имейл адресът е правилен.
    - Ако имейл адресът на потребителите не е зададен тук, след това създайте примерно предупреждение за този потребител, който кара синхронизирането на този потребителски акаунт от потребителски профили на SharePoint към тази колекция от сайтове.
 
2. Имейл от работни потоци се изпращат на администраторите на колекцията от сайтове, но не и на други потребители и вижте грешка **HTTP забранено <span>https https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.utility.SendEmail**.
 

    Вижте [Отказан достъп, когато изпращате имейл до група на SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Също така проверете дали **функцията** ограничен достъп потребителски разрешение заключване режим колекция не е активен.


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft Flow в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


