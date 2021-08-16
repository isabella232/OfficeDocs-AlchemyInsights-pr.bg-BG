---
title: Коригиране Microsoft 365 приложения Съжаляваме, че имаме съобщение за временни проблеми със сървъра
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021585"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Коригиране на Microsoft 365 "За съжаление, имаме временни проблеми със сървъра"

Ако получите това съобщение, опитайте следното:

1. Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че не блокират достъпа до интернет Microsoft 365 приложения. Вижте [ДИАПАЗОНИ на URL адреси и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете на **Стартиране**  >  **на изпълнение** и след това въведете **services.msc**. Уверете се, че всички услуги по-долу се изпълняват:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга "Списък на мрежата"
    - Информираност за местоположението на мрежата
    - Windows Регистър на събитията

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:

**sfc /scannow**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно" грешка, когато активирате](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).