---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739482"
---
# <a name="how-to-disable-external-groups"></a>Как да забраните външни групи

Yammer външни съобщения се прилага Exchange транспортни правила (ETRs), набор от проактивни контроли за предотвратяване на споделяне на фирмени информация. За да ограничите потребителите от създаване на външни групи, трябва да конфигурирате транспорт правило за Exchange (ETR) и след това конфигурирайте Yammer да използвате Exchange транспорт правило за блокиране на външни съобщения.
  
След като сте създали правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR да приложите в Yammer:
  
- Влезте в Yammer като проверен администратор и в центъра за администриране на **yammer**отидете на C **съдържание и настройките за защита на \> защитата.**

- Под **външни съобщения**изберете **прилагане на Exchange Online Exchange правила за транспорт (etrs) в Yammer.**

- Изберете **Запиши**.

За повече информация вижте [забраняване на външни съобщения в Yammer мрежа](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  