---
title: Класически отчети на регистрационния файл за проверка на SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992607"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Регистрационни файлове за проверка на SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Регистрационни файлове на SharePoint класически проверка

СПО наследени одит е мигрирал към единни проверка регистрационен файл. Всички проспо стари одиторски отчети сега ще се захранва чрез IT и стари одит сигнали са мигрирали към програмата.

Основни промени:

* Почистването не е налично като възможност.
* Избирането на конкретни събития за проверка не е налично. Вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, налични по подразбиране.
* Опцията за **местоположение** под **персонализирани отчети** не е налична.
* Опцията за **Отваряне или изтегляне на документи** събития не е налична.

[Конфигуриране на настройките за проверка за колекция от сайтове](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint и OneDrive съвременни единни проверка регистрационни файлове от съответствие

* [Включване/изключване на единно регистриране на проверка](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Не се изисква допълнителна конфигурация в SharePoint или OneDrive.

Използвайте проверка регистриране на търсене, за да проверите активността на файлове, папки, потребител (и), разрешения:

* [Дейности с файлове и страници](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Дейности в папките](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Споделяне и достъп до дейности по заявка](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Дейности по синхронизация](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Дейности по администриране на сайта](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл на проверката](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
