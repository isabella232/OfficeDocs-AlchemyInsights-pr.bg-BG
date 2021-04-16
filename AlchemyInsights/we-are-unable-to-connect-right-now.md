---
title: Проблем с активирането – в момента не можем да се свържем
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806431"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Коригиране на съобщението "Не можем да се свържем в момента" на приложенията на Microsoft 365

Ако получите това съобщение, опитайте следното:

1. Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че не блокират достъпа до интернет до приложенията на Microsoft 365. Вижте [Диапазони от URL и IP адреси на Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете на **Стартиране**  >  **на изпълнение** и след това въведете **services.msc**. Уверете се, че всички услуги по-долу се изпълняват:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга "Списък на мрежата"
    - Информираност за местоположението на мрежата
    - Регистър на събитията в Windows

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:

**sfc /scannow**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно" грешка, когато активирате Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).