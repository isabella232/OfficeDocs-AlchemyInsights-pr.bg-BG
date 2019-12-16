---
title: Имейл работният поток не се изпраща
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049362"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Имейл работен поток не се изпраща за списък или библиотека на SharePoint

1. Имейл от работни потоци не се изпращат до всички потребители или само конкретни потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.

    Проверете дали потребителят съществува в групата " **всички хора** разрешения" (списък с потребителски информация) за тази колекция от сайтове.  Примерен Директен URL адрес:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/kari.Lap? Членове на групата = 0

    - Ако потребителят не съществува, уверете се, че потребителят е влязъл в страницата. 
    - Ако е външен потребител, уверете се, че поканата им е приета.
    - Ако потребителят съществува в групата с разрешения, уверете се, че имейл адресът е правилен.
    - Ако потребителят имейл адрес не е зададен тук, след това създайте примерен сигнал за този потребител, който принуждава синхронизирането на този потребителски акаунт от потребителски профили на SharePoint в тази колекция от сайтове.
 
2. Имейл от работни потоци се изпращат на администраторите на колекцията от сайтове, но не и на други потребители и да видите грешка **http забранено да <span>HTTPS:</span>//_vti_bin/клиент.ксвк.сп.утилитиес.утилити.сендемаил**.
 

    Вижте [достъп отказан, когато изпращате имейл до група на SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Също така Уверете се, че **ограничен достъп потребител разрешение режим заключване** сайт колекция не е активен.


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft Flow в SharePoint online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


