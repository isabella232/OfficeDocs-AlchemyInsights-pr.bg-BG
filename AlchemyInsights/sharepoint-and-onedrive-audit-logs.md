---
title: Класически отчети на регистрационния файл за проверка на SharePoint
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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741954"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Регистрационни файлове за проверка на SharePoint и OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Класически регистрационни файлове за проверка на SharePoint

SPO одитът на наследството е пренесен в единни регистрационен файл за проверка (UAL). Всички sPO одитни доклади сега ще бъде захранван чрез UAL и стари одит сигнали са пренесени в UAL.

Основни промени:

* Подстригването НЕ е налично като възможност.
* Изборът на конкретни събития за проверка НЕ е наличен. Вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитирани събития, налични по подразбиране.
* Опцията **Местоположение** под **Персонализирани отчети** НЕ е налична.
* Опцията **За отваряне или изтегляне на документи** събития не е налична.

[Конфигуриране на настройките за проверка за колекция от сайтове](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Регистрационнифайлове за проверка на SharePoint и OneDrive съвременни единни проверки от съответствието

* [Включване/изключване на регистрирането на единни одит](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Не се изисква допълнителна конфигурация в SharePoint или OneDrive.

Използвайте проверка на регистрирането търсене, за да проверите дейността на файловете, папките, потребителите, разрешенията:

* [Дейности по файловете и страниците](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Дейности в папки](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Дейности за споделяне и достъп до заявки](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Дейности по синхронизиране](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Административни дейности на обекта](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

За повече информация как да извлечете тези събития вижте [Търсене в регистрационния файл за проверка](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
