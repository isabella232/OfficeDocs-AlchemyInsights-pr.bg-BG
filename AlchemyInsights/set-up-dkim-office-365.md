---
title: Настройка на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108545"
---
# <a name="setup-dkim"></a>Настройка на DKIM

Пълните инструкции за конфигуриране на DKIM за домейни по избор в Microsoft 365 са [тук.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. За **всеки** домейн по избор трябва да създадете **два** DKIM CNAME записа в DNS хостинг услугата на вашия домейн (обикновено регистратор на домейни). Например contoso.com и fourthcoffee.com четири DKIM CNAME записа: два за contoso.com и два за fourthcoffee.com.

   DKIM CNAME записите за **всеки домейн** по избор използват следните формати:

   - **Име на хоста:**`selector1._domainkey.<CustomDomain>`

     **Сочи към адрес или стойност:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Име на хоста:**`selector2._domainkey.<CustomDomain>`

     **Сочи към адрес или стойност:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> е текстът отляво на персонализирания MX запис за домейна по избор `.mail.protection.outlook.com` (например `contoso-com` за домейна contoso.com). \<InitialDomain\>е домейнът, който сте използвали, когато сте се записали за Microsoft 365 (например contoso.onmicrosoft.com).

2. След като създадете CNAME записите за вашите домейни по избор, изпълнете следните инструкции:

   a. [влезте, за Microsoft 365 със](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) своя работен или учебен акаунт.

   b. Изберете иконата за стартиране на приложения в горния ляв ъгъл и изберете **Администратор**.

   c. В навигацията в долния ляв ъгъл **разгънете Администратор** и **Exchange**.

   d. Отидете на **Защита**  >  **DKIM**.

   e. Изберете домейна и след това изберете **Разреши** **за подписване на съобщения за този домейн с DKIM подписи**. Повторете тази стъпка за всеки домейн по избор.
