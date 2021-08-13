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
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093795"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничаване на достъпа в SharePoint или OneDrive

Има много начини за ограничаване на достъпа до SharePoint онлайн/OneDrive услуги. Тези различни методи за ограничаване на достъпа са описани по-долу. 

**Ограничение за разрешение**

В SharePoint онлайн и OneDrive за бизнеса ограничаваме достъпа до елементи като сайтове, файлове и папки, като предоставяме достъп само на тези групи/лица, които трябва да имат достъп.

- [Персонализиране на разрешения за SharePoint списък или библиотека](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Персонализиране SharePoint разрешения за сайт](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Промяна на разрешенията в подпапка](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Управление на достъпа от неувършени устройства](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Като SharePoint или глобален администратор, можете да блокирате или ограничите достъпа до съдържание на SharePoint и OneDrive от неудържими устройства (тези, които не са хибридни AD, присъединени или съвместими в Intune).

**Ограничение за местоположение в мрежата**

Като ИТ администратор можете да управлявате достъпа до SharePoint и OneDrive въз основа на определени мрежови местоположения, на които имате доверие. Това е известно също като правила, базирани на местоположение. За повече информация вижте Управление на [достъпа до SharePoint онлайн и OneDrive данни въз основа на местоположението на мрежата](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение за заключване на сайт** 

В SharePoint онлайн имате възможност да заключите колекция от сайтове, така че никой да няма достъп. Това е зададено чрез PowerShell [и SharePoint за](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) онлайн управление с помощта на [свойството Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ограничаване на потребителите да създават сайтове или подсайтове**

Като администратор на SharePoint или глобален администратор, можете да позволите на вашите потребители да създават и администрират свои собствени сайтове на SharePoint, да определят какъв тип сайтове могат да създават и да задават местоположението на сайтовете. За повече информация вижте Управление на [създаването на сайтове в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

