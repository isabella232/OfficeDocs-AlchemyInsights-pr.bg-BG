---
title: Внедряване на Win32 приложението
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461741"
---
# <a name="intune-win32-app-deployment"></a>Внедряване на Win32 приложението

Приложението Microsoft позволява Win32 приложения, включително, но не само MSI и. EXE за разполагане на устройства с Windows 10. Използваният механизъм за разполагане изисква разширеното разширение за управление (IME) да присъства на целевото устройство. IME ще се инсталира автоматично като резултат от насочване на скрипт на PowerShell или разполагане на Win32 към потребител/устройство.

Има и набор от предварителни изисквания, които трябва да бъдат изпълнени, за да се разположи Win32 приложенията, които включват:

- Поддържани платформи: Windows 10 версия 1607 или по-нова (версии Enterprise, Pro и Education).
- Поддържана архитектура: x86 и x64.
- Управление на устройства: пад присъединен и автоматично записване (включително хибриден домейн, присъединен към и автоматично записване на групови правила).
- Формат на пакета приложения: **intunewin**  файл, подготвен от [инструмента за подготовка на съдържание за Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Ограничения
    - Максимален размер: 8GB.
    - Неподдържана архитектура: ARMs.

Прегледайте документа "[Добавяне, даване и следене на приложението Win32 в Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" за информация относно тези стъпки.

Подробни данни за разполагането на приложения за отстраняване на неизправности в Windows, включително Win32 приложенията, могат да бъдат преглеждани в следните документи

- [Отстраняване на проблеми с инсталирането на приложения](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Отстраняване на неизправности при Win32 приложения](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)