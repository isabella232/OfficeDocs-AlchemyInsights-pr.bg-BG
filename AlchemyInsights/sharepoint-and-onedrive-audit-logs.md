---
title: Класически отчети за проверка на SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509589"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Регистрационни файлове за проверка на SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Регистрационни файлове за класически проверки на SharePoint

SPO наследен одит е пренесена в единни регистрационен файл за проверка (UAL). Всички SPO доклади за наследени одити сега ще се устояват чрез UAL, а наследените одиторски сигнали са били мигрирани към UAL.

Основни промени:

* Подстригването НЕ е налично като възможност.
* Изборът на конкретни събития за проверка НЕ е наличен. Вижте [този документ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) за пълен списък на проверените събития, налични по подразбиране.
* Опцията **"Местоположение"** под **Персонализирани отчети** НЕ е налична.
* Опцията **"Отваряне или изтегляне на събития на документи"** НЕ е налична.

[Конфигуриране на настройките за проверка за колекция от сайтове](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint и OneDrive съвременните единни регистрационни файлове за проверка от съответствието

* [Включване/изключване на регистриране на унифициран одит](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Не се изисква допълнителна конфигурация в SharePoint или OneDrive.

Използвайте търсене на регистриране на проверка, за да проверите дейността на файловете, папките, потребителите, разрешенията:

* [Дейности на файлове и страници](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Дейности на папки](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Дейности за споделяне и достъп до заявки](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Дейности по синхронизация](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Дейности по администриране на сайта](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

За повече информация как да извлечете тези събития вижте [Търсене в регистрационния файл за проверка](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
