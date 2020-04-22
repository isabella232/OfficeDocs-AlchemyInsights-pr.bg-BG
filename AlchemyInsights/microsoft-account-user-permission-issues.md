---
title: Отстраняване на проблем - Потребителят не е намерен в директорията
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702727"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Отстраняване на проблем - Потребителят не е намерен в директорията

Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в директорията, опитайте отново, когато тип на проблема не е в директорията.

Следните стъпки могат да бъдат завършени, за да отстраните проблема.

- Уверете се, че акаунтът, който е приел поканата за имейл, е същият, който се използва за влизане в по-късно. Уверете се, че потребителят използва същия акаунт, за да приеме поканата и влезе в сайта. 

За повече информация [вж.</a> ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Намерете всеки сайт(и), в който потребителят получава грешката. 

Добавете "/_layouts/15/people.aspx/членска група=0" (в рамките на двойните кавички) към края на URL адреса на сайта. 

Пример: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Изберете потребителя от списъка.

- Щракнете върху **Премахване на потребителски разрешения** от лентата. 
-  Добавете обратно потребителя и изпрати покана та на потребителя.

