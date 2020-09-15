---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700444"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничаване на достъпа в SharePoint или OneDrive

Има много начини да ограничите достъпа до услугите на SharePoint online/OneDrive. По-долу са описани различните методи за ограничаване на достъпа. 

**Ограничения за разрешения**

В SharePoint online и OneDrive за бизнеса ние ограничаваме достъпа до елементи като сайтове, файлове и папки само чрез предоставяне на достъп до тези групи/лица, които трябва да имат достъп.

- [Персонализиране на разрешения за списък или библиотека на SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Персонализиране на разрешения за сайт на SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Промяна на разрешенията в подпапка](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Управление на достъпа от неуправлявани устройства](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Като администратор на SharePoint или глобален, можете да блокирате или да ограничите достъпа до съдържание на SharePoint и OneDrive от неуправлявани устройства (тези, които не са хибридни, се присъединили или съобразени в съответствие).

**Ограничение на мрежовото местоположение**

Като ИТ администратор, можете да управлявате достъпа до ресурси на SharePoint и OneDrive на базата на определени местоположения в мрежата, на които се доверявате. Това е известно също като правила, базирани на местоположение. За повече информация вижте [управление на достъпа до данните от SharePoint online и OneDrive въз основа на мрежовото местоположение](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение за заключване на сайта** 

В SharePoint online имате възможност да заключите колекция от сайтове, така че никой да няма достъп до тях. Това е зададено чрез PowerShell и [обвивката за управление на SharePoint online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) чрез свойството [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ограничаване на потребителите от създаване на сайтове или подсайтове**

Като администратор на SharePoint или глобален администратор, можете да позволите на потребителите да създават и администрират собствените си сайтове на SharePoint, да определят какви видове сайтове могат да създават и да указват местоположението на сайтовете. За повече информация вижте [управление на създаването на сайтове в SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

