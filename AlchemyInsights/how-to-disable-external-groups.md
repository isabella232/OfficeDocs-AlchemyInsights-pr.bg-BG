---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720757"
---
# <a name="how-to-disable-external-groups"></a>Как да забраните външни групи

Yammer външни съобщения прилага Exchange транспортни правила (ETRs), набор от проактивни контроли за предотвратяване на споделянето на информация за фирмата. За да ограничите потребителите от създаване на външни групи, трябва да конфигурирате Exchange транспортно правило (ETR) и след това конфигурирате Yammer да използва Exchange транспорт правило за блокиране на външни съобщения.
  
След като сте създали правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR да се прилагат в Yammer:
  
- Влезте в Yammer като проверен администратор и в центъра за администриране на **Yammer**отидете на C **съдържание и \> сигурност настройки.**

- Под **Външни съобщения**изберете Прилагане на exchange Online Exchange транспорт правила **(ETRs) в Yammer.**

- Изберете **Записване**.

За повече информация вижте [Забраняване на външни съобщения в yammer мрежа](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  