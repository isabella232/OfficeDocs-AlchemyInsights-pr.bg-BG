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
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015609"
---
# <a name="how-to-disable-external-groups"></a>Как да забраните външни групи

Yammer външни съобщения се прилага Exchange транспортни правила (ETRs), набор от проактивни контроли, за да не се споделя информация за фирмата. За да ограничите потребителите да създават външни групи, трябва да конфигурирате транспортно правило на Exchange (ETR) и след това да конфигурирате Yammer, за да използвате правилото Exchange Транспорт, за да блокирате външните съобщения.
  
След като сте създали правило в центъра за Exchange Online, следвайте тези стъпки, за да зададете ETR да се прилага в Yammer:
  
- Влезте в Yammer като проверен администратор и в **центъра за администриране на Yammer** отидете на C Content and Security security **\> Настройки.**

- Под **Външни съобщения изберете** Налагане на Exchange Online Exchange транспортни правила **(ETRs) в Yammer.**

- Изберете **Запиши**.

За повече информация вижте [Забраняване на външни съобщения в Yammer мрежа](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  