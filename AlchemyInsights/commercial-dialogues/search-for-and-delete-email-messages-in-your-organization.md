---
title: Търсене и изтриване на имейл съобщения във вашата организация
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743777"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Търсене и изтриване на имейл съобщения във вашата организация

Изпълнете следните стъпки:

1. Ако не сте глобален администратор, за да търсите съобщения, Вашият акаунт трябва да бъде добавен към **ролевата група "Диспечер на откриване** на електронни данни" или към **ролята за управление на търсенето в съответствие**. За да изтриете съобщения, ще трябва да се присъедините към **ролевата група за управление на организацията** или към **ролята за управление на търсенето и изчистването**. Разрешенията за тези роли се присвояват в [центъра за съответствие на & за защита.](https://protection.office.com)
2. [Създаване на търсене на съдържание](https://docs.microsoft.com/office365/securitycompliance/content-search) , за да се намери съобщението за изтриване.
3. [Свързване към центъра за администриране на & на съвместимост на PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ако използвате многофакторно удостоверяване, вижте следните инструкции: [Свързване към центъра за сигурност &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Изтрийте съобщението: изпълнете `New-ComplianceSearchAction` кратката команда, за да изтриете съобщението. Изтритите съобщения се преместват в папката "Възстановими елементи" на потребителя. За примерна команда вижте [стъпка 3: Изтрийте съобщението.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
