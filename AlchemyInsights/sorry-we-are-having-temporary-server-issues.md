---
title: Фиксиране на приложения на Office Съжаляваме, имаме временно съобщение за проблеми със сървъра
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627979"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Определяне на приложенията на Office "Съжаляваме, имаме временен сървър проблеми" съобщение

Ако получите това съобщение, опитайте следното:

1. Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да потвърдите, че те не блокират интернет достъпа до приложенията на Office. Вижте [URL адресите на Office 365 и IP адресните диапазони](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете на **Стартирай** > **, след**което въведете **Services. msc**. Уверете се, че всички следните услуги се изпълняват:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга за мрежови списъци
    - Осведоменост за местоположението в мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:

**сок/скансега**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка при активиране на Office от Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).