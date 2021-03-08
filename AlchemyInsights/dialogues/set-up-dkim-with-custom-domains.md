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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523252"
---
# <a name="set-up-dkim-with-custom-domains"></a>Настройване на DKIM с домейни по избор

За всеки домейн по избор в DNS трябва да публикувате два CNAME записа. За да направите това, използвайте следния формат:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** е текстът отляво на **. mail.Protection.Outlook.com** в персонализирания MX запис за домейна по избор (например contoso-com за домейна **contoso.com**). **InitialDomain** е домейнът, който сте използвали, когато сте се записали за Office 365 (например **contoso.onmicrosoft.com**).

За повече информация за DNS записите вижте [Създаване на DNS записи при доставчик на DNS хостинг за Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).