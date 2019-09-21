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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068012"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Регистрационни файлове за проверка на SharePoint и OneDrive

**SharePoint и OneDrive съвременни единни проверка регистрационни файлове от съответствие**

- [Включване/изключване на единно регистриране на проверка](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Не се изисква допълнителна конфигурация в SharePoint или OneDrive.

- Използвайте проверка регистриране на търсене, за да проверите активността на файлове, папки, потребител (и), разрешения:

    - [Дейности с файлове и страници](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Дейности в папките](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Споделяне и достъп до дейности по заявка](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Дейности по синхронизация](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Дейности по администриране на сайта](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл на проверката](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Регистрационни файлове на SharePoint класически проверка**

Ние мигрират спо наследени проверка на единни проверка регистрационен файл. По същество това означава, че всички съществуващи доклади за одит на спо ще бъдат захранвани чрез програмата за проверка на данни, а стари одитни сигнали са мигрирали към него.

Основни промени:

- Почистването като възможност не е налично.
- Разделът, в който избирате конкретни събития за проверка, не е наличен. Моля, вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, налични по подразбиране.
- Опцията "местоположение" под **персонализирани отчети** не е налична. 
- "Отваряне или изтегляне на документи" събития не е налична. 

