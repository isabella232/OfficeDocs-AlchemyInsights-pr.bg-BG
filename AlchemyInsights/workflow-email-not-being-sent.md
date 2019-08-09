---
title: Поток имейл не се изпраща
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
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270661"
---
# <a name="workflow-email-is-not-being-sent"></a>Поток имейл не се изпраща

1. Имейл от работни потоци, които не са изпратени до всички потребители или само определени потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.

    Проверете дали потребителят съществува в група за разрешения на **Всички хора** (списък с потребителска информация) за тази колекция от сайтове.  Проба директно URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Ако потребителят не съществува, се уверете, че потребителят е подписан в страницата. 
    - Ако е външен потребител, се уверете, че техните покана е била приета.
    - Ако потребителят съществува в групата разрешения, се уверете, че имейл адресът е правилен.
    - Ако потребителите имейл адрес не е настроен тук, след това създайте примерно предупреждение за този потребител, който принуждава синхронизиране на този акаунт от потребителски профили на SharePoint към тази колекция от сайтове.
 
2. Имейл от работни потоци са изпратени до администраторите на колекцията сайтове, но не на други потребители и видите грешка **HTTP Забранения да <spam> <spam> ** <spam> <spam>.
 

    Вижте [Отказан достъп, когато се изпраща имейл до групите](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Също така Уверете се че функция на колекция сайтове **ограничен достъп потребител разрешение lockdown режим** не е активен.


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft поток в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


