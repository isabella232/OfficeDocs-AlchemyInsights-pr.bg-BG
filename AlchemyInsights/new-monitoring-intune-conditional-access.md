---
title: Монитор intune conditional Access
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025491"
---
# <a name="monitor-intune-conditional-access"></a>Монитор intune conditional Access

Потребителите, които са насочени към условен достъп, ще получат имейл с известие, ако не отговарят на изискванията за достъп на вашата организация. За да отстраните проблема, ви препоръчваме едно или повече от следните решения:

1. Ако се предполага, че устройството е записано, посъветвайте потребителя да отиде в приложението Company Portal и се уверете, че се показва в Company Portal. Ако това не стане, потребителят трябва да запише устройството.
1. В портала на Azure отидете на **Съответствие на устройството с Intune**  >  . 
1. За да прегледате отчета за съответствие на устройството си, за да проверите дали устройството на потребителя е маркирано като съвместимо, под **Монитор** щракнете върху Съответствие **на устройството.**
1. В портала на Azure отидете на **Съответствие на устройството с Intune**  >  . Под **Управление щракнете** върху **Правила**. В списъка с правила за съответствие се уверете, че профилът е присвоен на устройството на вашия потребител. Ако не е присвоен профил, Intune няма да може да потвърди състоянието на съответствие на устройството.
1. Редактиране на задачата за условен достъп на потребителя.
1. В портала на Azure отидете до Правила за условен достъп на **Intune**, изберете  >    >  правила от списъка и щракнете **върху Потребители и групи**.
1. За да насочите определени правила към някого, добавете ги към **списъка Включи**. За да сте сигурни, че дадено лице е пропуснато от правилата, добавете го в **списъка Изключване**.

**Полезни връзки:**

- [Общ преглед на съответствието на устройствата](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Отстраняване на неизправности в CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Правила за отстраняване на неизправности](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Наблюдение на съответствието на устройството с Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Тези стъпки са полезни само при отстраняването на Azure Active Directory функция Условен достъп. Възможно е също да поставите под карантина устройство, блокиращо достъпа му до имейл с Exchange правила. Повече информация за управлението Exchange устройства можете да намерите [**тук.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
