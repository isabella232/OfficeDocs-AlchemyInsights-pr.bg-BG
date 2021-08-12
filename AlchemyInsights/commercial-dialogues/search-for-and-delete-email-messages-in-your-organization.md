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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948872"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Търсене и изтриване на имейл съобщения във вашата организация

Изпълнете следните стъпки:

1. Ако не сте глобален администратор, за да търсите съобщения, вашият акаунт трябва да бъде добавен към **ролевата група на диспечера** за откриване на електронни данни или ролята **за управление на търсенето на съответствие.** За да изтриете съобщения, ще трябва да се присъедините към ролевата група **"Управление** на организацията" или **ролята за управление на търсенето и прочистването**. Разрешенията за тези роли се присвояват в центъра за [& съответствие.](https://protection.office.com)
2. [Създайте търсене на съдържание,](https://docs.microsoft.com/office365/securitycompliance/content-search) за да намерите съобщението за изтриване.
3. [Свързване на центъра за & за защита на PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ако използвате многофакторно удостоверяване, вижте следните инструкции: Свързване центъра за & съответствие на PowerShell с [помощта на многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Изтрийте съобщението: изпълнете `New-ComplianceSearchAction` кратката команда, за да изтриете съобщението. Изтритите съобщения се преместват в папката "Възстановими елементи" на потребителя. Например команда вижте Стъпка [3: Изтриване на съобщението.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
