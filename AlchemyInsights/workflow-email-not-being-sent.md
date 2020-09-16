---
title: Имейлът на работния поток не се изпраща
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
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748978"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Имейл на работен поток не се изпраща за списък или библиотека на SharePoint

1. Имейлът от работните потоци не се изпраща до всички потребители или само до определени потребители или виждате грешката, **която имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.

    Проверете дали потребителят съществува в групата " **всички** разрешения за хора" (списък с информация за потребителите) за тази колекция от сайтове.  Примерен Директен URL адрес: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Ако потребителят не съществува, уверете се, че потребителят е влязъл в страницата. 
    - Ако е външен потребител, уверете се, че поканата е приета.
    - Ако потребителят съществува в групата "разрешения", уверете се, че имейл адресът е правилен.
    - Ако имейл адресът на потребителите не е зададен тук, тогава Създайте примерно известие за този потребител, което принуждава синхронизирането на този потребителски акаунт от потребителските профили на SharePoint в тази колекция от сайтове.
 
2. Имейлите от работните потоци се изпращат до администраторите на колекцията от сайтове, но не и с други потребители и ще видите грешката, която **http е забранена за <span>HTTPS:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.SendEmail**.
 

    Вижте [отказан достъп, когато изпращате имейл до група на SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Също така се уверете, че функцията за **заключване на потребителските разрешения за ограничения на достъпа на потребители**


## <a name="related-topics"></a>Сродни теми
Искате да изпробвате Microsoft Flow в SharePoint online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


