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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509373"
---
# <a name="setup-dkim"></a>Настройка на DKIM

Пълните инструкции за конфигуриране на DKIM за потребителски домейни в Microsoft 365 са [тук.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. За **всеки** потребителски домейн трябва да създадете **два** DKIM CNAME записа в DNS хостинг услугата на домейна ви (обикновено регистратор на домейни). Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: два за contoso.com и два за fourthcoffee.com.

   DKIM CNAME записи за **всеки** домейн използва следните формати:

   - **Име на хост**:`selector1._domainkey.<CustomDomain>`

     **Точки за адрес или стойност:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **1000**000 евро

   - **Име на хост**:`selector2._domainkey.<CustomDomain>`

     **Точки за адрес или стойност:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **1000**000 евро

   \<DomainGUID\>е текстът отляво на `.mail.protection.outlook.com` персонализирания MX запис за домейна по избор (например `contoso-com` за домейна contoso.com). \<InitialDomain\>е домейнът, който сте използвали при регистрация за Microsoft 365 (например contoso.onmicrosoft.com).

2. След като създадете записите CNAME за вашите потребителски домейни, изпълнете следните инструкции:

   A. [влезте в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с вашия служебен или учебен акаунт.

   B. Изберете иконата на стартера на приложението в горния ляв ъгъл и изберете **Администриране**.

   C. В навигацията в долния ляв ъгъл разгънете **Администратор** и изберете **Exchange**.

   D. Отидете на **Защита**  >  **DKIM**.

   E. Изберете домейна и след това изберете **Разрешаване** за **подписване на съобщения за този домейн с DKIM подписи**. Повторете тази стъпка за всеки домейн по избор.
