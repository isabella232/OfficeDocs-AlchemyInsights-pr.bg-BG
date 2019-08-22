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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530851"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Поток имейл не се изпраща за SharePoint списък или библиотека

1. Имейл от работни потоци, които не са изпратени до всички потребители или само определени потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.

    Проверете дали потребителят съществува в група за разрешения на **Всички хора** (списък с потребителска информация) за тази колекция от сайтове.  Проба директно URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Ако потребителят не съществува, се уверете, че потребителят е подписан в страницата. 
    - Ако е външен потребител, се уверете, че техните покана е била приета.
    - Ако потребителят съществува в групата разрешения, се уверете, че имейл адресът е правилен.
    - Ако потребителите имейл адрес не е настроен тук, след това създайте примерно предупреждение за този потребител, който принуждава синхронизиране на този акаунт от потребителски профили на SharePoint към тази колекция от сайтове.
 
2. Имейл от работни потоци са изпратени до администраторите на колекцията сайтове, но не на други потребители и видите грешка **HTTP Забранения да <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Вижте [Отказан достъп, когато изпращате имейл на SharePoint група](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Също така Уверете се че функция на колекция сайтове **ограничен достъп потребител разрешение lockdown режим** не е активен.


## <a name="related-topics"></a>Сродни теми
Искате ли да опитате Microsoft поток в SharePoint Online?
- [Създаване на поток](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и поток](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


