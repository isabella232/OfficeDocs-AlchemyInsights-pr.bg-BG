---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750653"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничаване на достъпа в SharePoint или OneDrive

Има много начини за ограничаване на достъпа до услуги на SharePoint online/OneDrive. Тези различни методи за ограничаване на достъпа са описани по-долу. 

**Ограничение на разрешенията**

В SharePoint online и OneDrive за бизнес ограничаваме достъпа до елементи като сайтове, файлове и папки само чрез предоставяне на достъп до тези групи/лица, които трябва да имат достъп.

- [Персонализиране на разрешенията за списък или библиотека на SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Персонализиране на разрешенията на сайта на SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Промяна на разрешенията на подпапка](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Контрол на достъпа от неуправлявани устройства](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Като SharePoint или глобален администратор в Office 365, можете да блокирате или ограничите достъпа до съдържание на SharePoint и OneDrive от неуправлявани устройства (хибридни AD, Съединени или съвместими в InTune).

**Ограничаване на местоположението в мрежата**

Като ИТ администратор можете да контролирате достъпа до ресурси на SharePoint и OneDrive въз основа на дефинирани мрежови местоположения, на които имате доверие. Това е известно също като политика, базирана на местоположението. За повече информация вижте [контрол на достъпа до SharePoint online и OneDrive данни въз основа на мрежово местоположение](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение за заключване на сайта** 

В SharePoint online имате възможност да заключите колекция от сайтове, така че никой няма достъп. Това е зададено чрез PowerShell и [онлайн обвивката за управление на SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощта на свойството [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -заключване.

**Ограничаване на потребителите да създават сайтове или подстраници**

Като администратор на SharePoint или Office 365 глобален администратор можете да позволите на потребителите да създават и администрират собствени сайтове на SharePoint, да определят какъв вид сайтове могат да създават и да посочат местоположението на сайтовете. За повече информация вижте [управление на създаването на сайт в SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

