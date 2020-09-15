---
title: 1554 WinSock грешка 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698851"
---
# <a name="winsock-error-10061"></a>Winsock грешка 10061

Този код на грешка означава, че Microsoft не може да установи TCP сокет (връзка) с целевия хост. Най-вероятната причина за тази грешка е проблем с конфигурацията на вашата защитна стена. За да отстраните проблема, отметнете тези настройки:

- Проверете конфигурацията на вашата защитна стена с информацията в [диапазони от URL и IP адреси на Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ако грешката е конкретна за Exchange Online Protection (EOP), трябва да сте уведомили предварително за промяна на [IP адресите за Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Уверете се, че вашият доставчик на интернет (ISP) не блокира порта.

- Проверете настройките за смарт хост и целеви сървър във вашите конектори.

Имайте предвид, че Microsoft 365 не блокира *входящите* връзки по следния начин.
