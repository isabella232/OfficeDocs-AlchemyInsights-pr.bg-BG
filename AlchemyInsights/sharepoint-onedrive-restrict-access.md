---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692754"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничаване на достъпа в SharePoint или OneDrive

Има много начини за ограничаване на достъпа до услуги на SharePoint Online/OneDrive. Тези различни методи за ограничаване на достъпа са описани по-долу. 

**Ограничение на разрешенията**

В SharePoint Online и OneDrive за бизнес, ние ограничаваме достъпа до елементи като сайтове, файлове и папки само предоставяне на достъп до тези групи/лица, които трябва да имат достъп.

- [Персонализиране на разрешения за списък или библиотека на SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Персонализиране на разрешенията за сайт на SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Промяна на разрешенията в подпапка](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Управление на достъпа от неуправлявани устройства](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Като SharePoint или глобален администратор можете да блокирате или ограничите достъпа до sharePoint и OneDrive съдържание от неуправлявани устройства (тези, които не са хибридни AD се присъедини или съвместими в Intune).

**Ограничение за местоположение в мрежата**

Като ИТ администратор можете да контролирате достъпа до ресурси на SharePoint и OneDrive въз основа на определени мрежови местоположения, на които имате доверие. Това е известно още като правила, базирани на местоположението. За повече информация вижте [управление на достъпа до SharePoint Online и OneDrive данни въз основа на местоположението на мрежата](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение за заключване на сайта** 

В рамките на SharePoint Online имате възможност да заключите колекция от сайтове, така че никой няма достъп. Това е зададено чрез PowerShell и [онлайн обвивката за управление](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) на SharePoint с помощта на [свойството Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState .

**Ограничаване на потребителите от създаване на сайтове или подсайтове**

Като администратор на SharePoint или глобален администратор можете да позволите на вашите потребители да създават и администрират свои собствени сайтове на SharePoint, да определят какъв вид сайтове могат да създават и да зададете местоположението на сайтовете. За повече информация вижте [управление на създаването на сайт в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

