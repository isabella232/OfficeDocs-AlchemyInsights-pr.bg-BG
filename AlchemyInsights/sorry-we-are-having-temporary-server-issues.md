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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744625"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Коригиране на Microsoft 365 "За съжаление, имаме временни проблеми със сървъра"

Забележка: Ако използвате по-стара версия на Windows (например Windows 7 SP1, Windows Server 2008 R2), използвайте лесната корекция, за да [разрешите](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) TLS 1.2 по подразбиране. За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows.

Ако получите това съобщение, опитайте следното:

1. Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че не блокират достъпа до интернет Microsoft 365 приложения. Вижте [ДИАПАЗОНИ НА URL адреси и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Отидете на **Стартиране**  >  **на изпълнение** и след това въведете **services.msc**. Уверете се, че всички услуги по-долу се изпълняват:
    - Автоматична настройка на свързаните с мрежата устройства
    - Услуга "Списък на мрежата"
    - Информираност за местоположението на мрежата
    - Windows Регистър на събитията

Ако една от тези услуги не се изпълнява, опитайте да я стартирате. Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:

**sfc /scannow**

След като тази команда завърши, рестартирайте компютъра.

За подробна информация вижте ["За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно" грешка, когато активирате](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).