---
title: Коригиране на office приложения за съжаление, имаме временни сървър проблеми съобщение
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764106"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Коригиране на office приложения "За съжаление, имаме временни сървър проблеми"

Ако се появи това съобщение, опитайте следното:

1. Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те не блокират достъпа до интернет за приложенията на Office. Вижте [URL адреси и ip адреси.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Отидете на **Стартиране на** > **изпълнение**и след това въведете **services.msc**. Уверете се, че са всички следните услуги:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга за мрежов списък
    - Информираност за местоположението в мрежата
    - Регистър на събитията на Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:

**SFC /сканиране**

След като тази команда приключи, рестартирайте компютъра.

За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"грешка при активиране](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).