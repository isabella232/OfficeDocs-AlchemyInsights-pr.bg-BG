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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332296"
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
**Забележка:** **DomainGUID** е текстът отляво на **.mail.protection.outlook.com** в персонализирания MX запис за домейна по избор (например contoso-com за домейна **contoso.com**). **InitialDomain** е домейнът, който сте използвали, когато сте се записали за Office 365 **(например contoso.onmicrosoft.com**).

За повече информация относно DNS записите вижте Създаване на DNS записи при всеки доставчик на [DNS хостинг за Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)