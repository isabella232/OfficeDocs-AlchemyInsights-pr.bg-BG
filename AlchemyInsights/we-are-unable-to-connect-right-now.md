---
title: Проблем с активирането – в момента не можем да се свържем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725972"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Отстраняване на неуспешно свързване на приложенията на Microsoft 365

Ако получите това съобщение, опитайте следното:

1. Проверете защитната стена, антивирусния софтуер и настройките за прокси сървър, за да потвърдите, че не блокират достъпа до интернет за приложенията на Microsoft 365. Вижте [диапазони от URL и IP адреси на Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете на **Старт**  >  **Run**и след това въведете **Services. msc**. Уверете се, че се изпълняват следните услуги:
    - Автоматично настройване на свързаните с мрежата устройства
    - Услуга за списък с мрежи
    - Информиране за местоположения в мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем при стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:

**SFC за разлагане**

След като тази команда завърши, рестартирайте компютъра.

За по-подробна информация вижте ["за съжаление не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка, когато активирате Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).