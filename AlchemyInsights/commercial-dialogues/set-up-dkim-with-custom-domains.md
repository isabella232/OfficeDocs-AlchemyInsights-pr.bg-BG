---
title: Настройване на DKIM с домейни по избор
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994778"
---
# <a name="set-up-dkim-with-custom-domains"></a>Настройване на DKIM с домейни по избор

Трябва да публикувате два CNAME записа за всеки домейн по избор в DNS. За да направите това, използвайте следния формат:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** е текстът отляво на **.mail.protection.outlook.com** в персонализирания MX запис за домейна по избор (например contoso-com за **домейна contoso.com**). **InitialDomain** е домейнът, който сте използвали, когато сте се записали за Office 365 **(например contoso.onmicrosoft.com**).

За повече информация относно DNS записите вижте [Създаване на DNS записи при всеки доставчик на DNS хостинг за Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)