---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223701"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничаване на достъпа в SharePoint или OneDrive

Има много начини за ограничаване на достъпа до услуги SharePoint Online/OneDrive. Тези различни методи за ограничаване на достъп са описани по-долу. 

**Разрешение ограничение**

В SharePoint Online и OneDrive за бизнес ограничаваме достъпа до обекти като сайтове, файлове и папки чрез само предоставяне на достъп до тези групи/лица, които трябва да имат достъп.

- [Персонализиране на разрешения за списък на SharePoint или библиотека](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Персонализиране на разрешения на сайт на SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Промяна на разрешенията на подпапка](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Контрол на достъпа от неуправляван устройства](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Като SharePoint или глобален администратор в Office 365, можете да блокирате или да ограничите достъпа до съдържание на SharePoint и OneDrive от неуправляван устройства (тези не хибрид АД се присъединиха или съвместими в Intune).

**Мрежа местоположение ограничение**

Като ИТ администратор можете да контролирате достъпа до SharePoint и OneDrive ресурси, на базата на определени мрежови местоположения, които имате доверие. Това е също така известен като местоположение базирани политика. За повече информация моля вижте [контрол на достъпа до SharePoint Online и OneDrive данни, базиращи се на местоположение в мрежата](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничението за заключване на сайта** 

В рамките на SharePoint Online имате възможност за заключване надолу колекция сайтове, така че никой няма достъп. Това се задава чрез PowerShell и [SharePoint онлайн управление Шел](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) използване на [Набор-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState собственост.

**Ограничаване на потребителите да създават сайтове, или подсайтове**

Като администратор на SharePoint или Office 365 е глобален администратор, можете да позволите на вашите потребители създават и управляват свои собствени сайтове на SharePoint, определи какви сайтове те могат да създават и Задайте местоположението на обектите. За повече информация моля вижте [управление създаването на сайт в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

