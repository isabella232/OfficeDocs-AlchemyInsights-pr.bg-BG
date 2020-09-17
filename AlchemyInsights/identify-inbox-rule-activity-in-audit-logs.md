---
title: Идентифициране на дейността с правила за папка "Входящи" в регистрационни файлове за проверка
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779040"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Идентифициране на дейността с правила за папка "Входящи" в регистрационни файлове за проверка

Можете да използвате функцията за търсене в регистрационния файл за проверка в центъра за защита на & на Microsoft 365, за да преглеждате събития за правилата за входящи (създаване, модифициране и изтриване на правила за входящи).

1. Влезте в центъра за [съответствие на & на Microsoft 365](https://protection.office.com/).

2. Отидете на страницата **Search**за  >  **търсене в регистрационния файл за проверка** на търсенето.

3. Изберете диапазона от дати в полетата " **Начална дата** " и " **крайна дата** ".

4. Под **дейности за пощенска кутия на Exchange**Проверете дали полето **дейности** е зададено на " **InboxRule" Създаване/промяна/разрешаване/забраняване на правило за папка "Входящи"**.

5. Щракнете върху **търсене**.

В резултатите изберете запис за проверка. В изплаващо за подробни данни щракнете върху **повече информация**. В полето **параметри** се показва информация за настройките на правилото за папка "Входящи".

За повече информация вижте [определяне дали потребителят е създал правило за папка "Входящи"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
