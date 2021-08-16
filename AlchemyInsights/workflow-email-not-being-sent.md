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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072509"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Имейлът на работен поток не се изпраща за SharePoint списък или библиотека

1. Имейлът от работни потоци не се изпраща до всички потребители или само до определени потребители или виждате грешката Имейл съобщението не може да бъде изпратено. Уверете се, че имейлът **има валиден получател**.

    Проверете дали потребителят съществува в групата разрешения **"Всички хора"** (списък с потребителски данни) за тази колекция от сайтове.  Примерен директен URL адрес: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ако потребителят не съществува, уверете се, че потребителят е влезли в страницата. 
    - Ако е външен потребител, уверете се, че поканата му е приета.
    - Ако потребителят съществува в групата разрешения, уверете се, че имейл адресът е правилен.
    - Ако имейл адресът на потребителите не е зададен тук, създайте примерно известие за този потребител, което принуждава синхронизирането на този потребителски акаунт от потребителските профили на SharePoint към тази колекция от сайтове.
 
2. Имейлите от работни потоци се изпращат до администраторите на колекцията от сайтове, но не и до други потребители и виждат грешката HTTP Забранена за **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Вижте [Отказан достъп, когато изпращате имейл до SharePoint група](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Също така проверете дали функцията за колекция от сайтове на колекция от **сайтове в режим** на блокиране на разрешения с ограничен достъп не е активна.


## <a name="related-topics"></a>Сродни теми
Искате да изпробвате Microsoft Flow в SharePoint Онлайн?
- [Създаване на Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


