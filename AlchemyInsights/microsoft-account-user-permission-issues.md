---
title: Проблем с отстраняването на неизправности – потребителят не е намерен в указателя
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098159"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Проблем с отстраняването на неизправности – потребителят не е намерен в указателя

Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в указателя, опитайте отново, където типът на проблема е Потребител, който не е в указателя.

Следващите стъпки могат да бъдат изпълнени, за да отстраните проблема.

- Уверете се, че акаунтът, който е приел поканата за имейл, е същият акаунт, който се използва за влизане по-късно. Уверете се, че потребителят използва същия акаунт, за да приеме поканата и да влезе в сайта. 

За повече информация вижте Как [да управлявате псевдоними за вашия акаунт в Microsoft, </a> за да управлявате Microsoft 365 влизане.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Отидете до всеки сайт(и), в който потребителят получава грешката. 

Добавете "/_layouts/15/people.aspx/membershipgroupid=0" (в рамките на двойните кавички) към края на URL адреса на сайта. 

Пример: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Изберете потребителя от списъка.

- Щракнете **върху Премахване на потребителски разрешения** от лентата. 
-  Добавете обратно потребителя и пренасищайте поканата на потребителя.

