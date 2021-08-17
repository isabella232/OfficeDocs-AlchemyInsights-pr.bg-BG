---
title: Идентифициране на дейността на правилото за папка "Входящи" в регистрационните файлове за проверка
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
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891284"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Идентифициране на дейността на правилото за папка "Входящи" в регистрационните файлове за проверка

Можете да използвате търсенето в регистрационния файл за проверка в Център за съответствие на Microsoft 365, за да видите събитията на правилото "Входящи" (създаване, промяна и изтриване на правила за папка "Входящи").

1. Изпълнете една от следните стъпки:
   - В Център за съответствие на Microsoft 365 отидете <https://compliance.microsoft.com> на Проверка **на** \> **решения**. Или, за да отидете директно на страницата **Проверка,** използвайте <https://compliance.microsoft.com/auditlogsearch> .
   - В портала Microsoft 365 Defender в <https://security.microsoft.com> отидете на **Проверка**. Или, за да отидете директно на страницата **Проверка,** използвайте <https://security.microsoft.com/auditlogsearch> .

2. В раздела **Търсене** на страницата **Проверка** конфигурирайте следните настройки:
   - **Диапазон от дата и** час: Изберете диапазона от дати/време в **полетата Начало** **и** Край.
   - **Дейности**: Изберете една или повече от следните стойности:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Актуализиране на правилата за папка "Входящи" от Outlook клиент**

3. Когато сте готови, щракнете върху **Търсене**. Дейностите се показват на новата страница **за търсене на** проверка.

4. Изберете дейност в резултатите, за да отворите допълнителното меню с подробни данни. Информация за настройките на правилото за папка "Входящи" се показва в **полето Параметри.**

За повече информация вижте Определяне [дали потребител е създал правило за папка "Входящи".](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
