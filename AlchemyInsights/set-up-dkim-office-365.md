---
title: Настройка на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645661"
---
# <a name="setup-dkim"></a>Настройка на DKIM

Пълните инструкции за конфигуриране на DKIM за персонализирани домейни в Microsoft 365 са [тук](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. За **всеки** персонализиран домейн трябва да създадете **два** DKIM CNAME записа на DNS хостинг услуга на домейна си (обикновено, регистраторът на домейни). Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: два за contoso.com и два за fourthcoffee.com.

   DKIM CNAME записи за **всеки** домейн използва следните формати:

   - **Име на хоста:**`selector1._domainkey.<CustomDomain>`

     **Точки за адрес или стойност:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Име на хоста:**`selector2._domainkey.<CustomDomain>`

     **Точки за адрес или стойност:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> е текст ът `.mail.protection.outlook.com` отляво на потребителски MX запис за домейна по избор (например `contoso-com` домейн contoso.com). \<InitialDomain\> е домейнът, който сте използвали, когато сте се регистрирали за Microsoft 365 (например contoso.onmicrosoft.com).

2. След като сте създали CNAME записи за вашите персонализирани домейни, изпълнете следните инструкции:

   A. [влезете в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с вашия служебен или учебен акаунт.

   B. Изберете иконата за стартиране на приложения в горния ляв ъгъл и изберете **Администратор**.

   C. В долната лява навигация разгънете **Администратор** и изберете **Exchange**.

   D. Отидете на **Защита** > **DKIM**.

   E. Изберете домейна и след това изберете **Разрешаване** за Подписване на **съобщения за този домейн с DKIM подписи**. Повторете тази стъпка за всеки персонализиран домейн.
