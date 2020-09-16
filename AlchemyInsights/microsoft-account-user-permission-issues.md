---
title: Отстраняване на проблема – потребителят не е намерен в указателя
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725396"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Отстраняване на проблема – потребителят не е намерен в указателя

Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в указателя, опитайте отново, където типът на проблема е потребител, който не е в справочния указател.

Можете да изпълните следните стъпки, за да отстраните проблема.

- Уверете се, че акаунтът, който е приел поканата за имейл, е същият акаунт, който се използва за влизане по-късно. Уверете се, че потребителят използва един и същ акаунт, за да приеме поканата и да влезе в сайта. 

За повече информация вижте [как да управлявате псевдоними за своя акаунт в Microsoft, </a> за да управлявате Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Отидете до всеки сайт (ове), в който потребителят получава грешката. 

Добавете "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойните кавички) в края на URL адреса на сайта. 

Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Изберете потребителя от списъка.

- Щракнете върху **Премахване на потребителските разрешения** от лентата. 
-  Добавете обратно потребителя и повторно изпратете поканата на потребителя.

