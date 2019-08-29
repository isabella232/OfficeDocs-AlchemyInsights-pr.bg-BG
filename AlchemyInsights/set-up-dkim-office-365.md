---
title: Настройка DKIM в Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666253"
---
# <a name="setup-dkim-in-office-365"></a>Настройка DKIM в Office 365

Пълни инструкции за конфигуриране DKIM за потребителски домейни в Office 365 са [тук](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. За **всеки** потребителски домейн трябва да създадете **две** DKIM CNAME записите в хостинг услугата за вашия домейн DNS (обикновено, регистраторът на домейни). Например contoso.com и fourthcoffee.com изисква четири DKIM CNAME записи: две за contoso.com и два за fourthcoffee.com.

   DKIM CNAME записи за **всеки** потребителски домейн използва следните формати:

   - **Име на хост**:`selector1._domainkey.<CustomDomain>`

     **Точки за адрес или стойност**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Име на хост**:`selector2._domainkey.<CustomDomain>`

     **Точки за адрес или стойност**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> е текст от ляво на `.mail.protection.outlook.com` в потребителски MX записа за собствен домейн (например, `contoso-com` за домейна contoso.com). \<InitialDomain\> е домейн сте използвали, когато сте се регистрирали за Office 365 (например, contoso.onmicrosoft.com).

2. След като сте създали CNAME записи за вашите потребителски домейни, изпълнете следните инструкции:

   a. [Влезте в Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с профила си работа или училище.

   б. Изберете иконата на стартера на ап в горния ляв и **администратор**.

   c. В долния ляв навигация разгънете **администратор** и изберете **Exchange**.

   d. Отидете на **защита** > **DKIM**.

   д. Изберете домейн и след това изберете **Разреши** за **знак за съобщенията за този домейн с DKIM подписи**. Повторете тази стъпка за всеки домейн.
