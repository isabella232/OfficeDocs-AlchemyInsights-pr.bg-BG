---
title: Поправяне на приложения на Microsoft 365 Съжаляваме, имаме съобщение за временен проблем със сървъра
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758234"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Поправяне на приложенията на Microsoft 365 "за съжаление, имаме съобщение за временен проблем със сървъра"

Ако получите това съобщение, опитайте следното:

1. Проверете защитната стена, антивирусния софтуер и настройките за прокси сървър, за да потвърдите, че не блокират достъпа до интернет за приложенията на Microsoft 365. Вижте [диапазони от URL и IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)адреси.

2. Отидете на **Старт**  >  **Run**и след това въведете **Services. msc**. Уверете се, че се изпълняват следните услуги:
    - Автоматично настройване на свързаните с мрежата устройства
    - Услуга за списък с мрежи
    - Информиране за местоположения в мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем при стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:

**SFC за разлагане**

След като тази команда завърши, рестартирайте компютъра.

За по-подробна информация вижте ["за съжаление не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка при активиране](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).