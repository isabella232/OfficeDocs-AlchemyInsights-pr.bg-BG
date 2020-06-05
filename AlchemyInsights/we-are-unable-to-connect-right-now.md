---
title: Активиране проблем - Ние не сме в състояние да се свържем точно сега
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581864"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Коригиране на microsoft 365 приложения "Ние не сме в състояние да се свържете в момента" съобщение

Ако получите това съобщение, опитайте следното:

1. Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да се уверите, че не блокират достъпа до интернет до приложенията на Microsoft 365. Вижте [URL адресите на Microsoft и диапазоните на IP адресите](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете в **Старт**  >  **изпълнение**и след това въведете **services.msc**. Уверете се, че всички услуги се изпълняват следните:
    - Автоматично настройване на свързани в мрежа устройства
    - Услуга за списък на мрежи
    - Осведоменост за местоположението на мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да го стартирате. Ако имате проблем при стартиране на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:

**SFC / сканиране**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["Съжаляваме, не можем да се свържем с профила ви. Опитайте отново по-късно"грешка, когато активирате Office от Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)