---
title: Поправяне на Приложения на Microsoft 365 Съжаляваме, имаме съобщение за временни проблеми със сървъра
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582692"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Коригиране на Microsoft 365 приложения "Съжаляваме, имаме временни проблеми със сървъра" съобщение

Ако получите това съобщение, опитайте следното:

1. Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да се уверите, че не блокират достъпа до интернет до приложенията на Microsoft 365. Вижте [URL адреси и диапазони на IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете в **Старт**  >  **изпълнение**и след това въведете **services.msc**. Уверете се, че всички услуги се изпълняват следните:
    - Автоматично настройване на свързани в мрежа устройства
    - Услуга за списък на мрежи
    - Осведоменост за местоположението на мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да го стартирате. Ако имате проблем при стартиране на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:

**SFC / сканиране**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["Съжаляваме, не можем да се свържем с профила ви. Моля, опитайте отново по-късно"грешка при активиране.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)