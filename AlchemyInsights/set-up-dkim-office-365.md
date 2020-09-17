---
title: Настройки на DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808696"
---
# <a name="setup-dkim"></a>Настройки на DKIM

Пълните инструкции за конфигуриране на DKIM за домейни по избор в Microsoft 365 са [тук](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. За **всеки** домейн по избор трябва да създадете **два** DKIM CNAME ЗАПИСА в услугата за DNS хостинг на вашия домейн (обикновено регистраторът на домейни). Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: две за contoso.com и две за fourthcoffee.com.

   DKIM CNAME Records за **всеки** домейн по избор използва следните формати:

   - **Име на хост**: `selector1._domainkey.<CustomDomain>`

     **Сочи към адрес или стойност**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Име на хост**: `selector2._domainkey.<CustomDomain>`

     **Сочи към адрес или стойност**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> е текстът отляво на `.mail.protection.outlook.com` в персонализирания MX запис за домейна по избор (например `contoso-com` за домейна contoso.com). \<InitialDomain\> е домейнът, който сте използвали, когато сте се записали за Microsoft 365 (например contoso.onmicrosoft.com).

2. След като сте създали CNAME записите за вашите домейни по избор, изпълнете следните инструкции:

   на. [Влезте в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) със своя служебен или учебен акаунт.

   b. Изберете иконата за стартиране на приложения в горния ляв ъгъл и изберете **администратор**.

   c. В навигацията в долния ляв ъгъл разгънете **администратор** и изберете **Exchange**.

   d. Отидете на **Protection**  >  **DKIM**за защита.

   e. Изберете домейна и след това изберете **Разрешаване** на **подписване на съобщения за този домейн с подписи на DKIM**. Повторете тази стъпка за всеки домейн по избор.
