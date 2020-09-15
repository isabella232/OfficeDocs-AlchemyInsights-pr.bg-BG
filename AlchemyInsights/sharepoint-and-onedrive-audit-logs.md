---
title: Класически отчети на регистрационни файлове за проверка на SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662197"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Регистрационни файлове за проверка на SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Регистрационни файлове за проверка на класическия SharePoint

За да бъде мигриран Архивът за един и същ регистър за проверка (изп). Всички наследени отчети за проверка на всички данни ще се захранват чрез изп и наследените сигнали за проверка са мигрирани към изп.

Клавишни промени:

* Изрязването не е достъпно като способност.
* Избирането на конкретни събития за проверка не е налично. Вижте [този документ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, които са налични по подразбиране.
* Опцията за **местоположение** под **персонализирани отчети** е недостъпна.
* Опцията за **Отваряне или изтегляне на документи** е недостъпна.

[Конфигуриране на настройки за проверка на колекция от сайтове](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Нови регистри за унифицирани проверки на SharePoint и OneDrive за съответствие

* [Включване/изключване на регистрирането на унифицирани проверки](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Не се изисква допълнителна конфигурация в SharePoint или OneDrive.

Използване на търсене в регистрационния файл за проверка, за да се провери дейността на файловете, папките, потребителите, разрешенията:

* [Дейности с файлове и страници](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Дейности с папки](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Дейности за споделяне и достъп до заявка](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Дейности за синхронизиране](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Дейности за администриране на сайт](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл за проверка](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
