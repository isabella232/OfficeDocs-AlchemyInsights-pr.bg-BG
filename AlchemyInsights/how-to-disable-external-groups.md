---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704117"
---
# <a name="how-to-disable-external-groups"></a>Как да забраните външни групи

Във външните съобщения на Yammer се прилагат транспортни правила на Exchange (ETR) – набор от proactive контроли за предотвратяване на споделянето на информация за фирмата. За да ограничите потребителите при създаването на външни групи, трябва да конфигурирате транспортно правило на Exchange (ETR) и след това да конфигурирате Yammer, за да използвате транспортното правило на Exchange, за да блокирате външни съобщения.
  
След като създадете правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR, което да приложите в Yammer:
  
- Влезте в Yammer като проверен администратор и в центъра за администриране на **Yammer**отидете на настройки за защита на **съдържание и защита \> .**

- Под **външни съобщения**изберете **налагане на вашите транспортни правила на Exchange Online за транспорт (ETR) в Yammer.**

- Изберете **Запиши**.

За повече информация вижте [забраняване на външни съобщения в мрежа на Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  