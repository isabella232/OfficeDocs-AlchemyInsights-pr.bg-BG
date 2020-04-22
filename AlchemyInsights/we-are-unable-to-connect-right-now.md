---
title: Проблем при активиране - Не можем да се свържем точно сега
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716161"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Определяне на office приложения "Не можем да се свържете в момента" съобщение

Ако се появи това съобщение, опитайте следното:

1. Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те не блокират достъпа до интернет за приложенията на Office. Вижте [url адреси те на Microsoft и ip адреси.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Отидете на **Стартиране на** > **изпълнение**и след това въведете **services.msc**. Уверете се, че са всички следните услуги:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга за мрежов списък
    - Информираност за местоположението в мрежата
    - Регистър на събитията на Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:

**SFC /сканиране**

След като тази команда приключи, рестартирайте компютъра.

За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"грешка при активиране на Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).