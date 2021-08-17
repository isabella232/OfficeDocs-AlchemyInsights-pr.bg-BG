---
title: 1554 Winsock грешка 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083219"
---
# <a name="winsock-error-10061"></a>Winsock грешка 10061

Този код на грешка означава, че Microsoft не е могъл да установи TCP сокет (връзка) с целевия хост. Най-вероятната причина за тази грешка е проблем с конфигурацията на защитната стена. За да коригирате проблема, проверете следните настройки:

- Проверка на конфигурацията на защитната стена с [информацията в Microsoft 365 диапазони от URL и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ако грешката е специфична за Exchange Online Protection (EOP), би трябвало преди това да сте били уведомени за промяна [на Exchange Online Protection IP адреси.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Уверете се, че вашият доставчик на интернет услуги (ISP) не блокира порта.

- Проверете настройките на интелигентния хост и целевия сървър във вашите конектори.

Обърнете внимание Microsoft 365 че не блокира *входящите* връзки по този начин.
