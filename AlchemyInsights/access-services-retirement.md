---
title: Оттегляне на услугите на Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938684"
---
# <a name="access-services-retirement"></a>Оттегляне на услугите на Access

Както първоначално обявихме в MC97576, през март 2017 г. и продължихме да комуникираме през изминалата година, Access Services се оттеглят. Следващата фаза в този процес ще бъде премахването на уеб бази данни на Access, които използват SharePoint списъци като тяхното основно място за съхранение на данни.

**Как това ме засяга?**

От юни 2019 г. ще спрем създаването на нови бази данни на Access в SharePoint Online и ще изключим услугата и всички останали приложения до април 2020 г.

**Какво трябва да направя, за да се подготвя за тази промяна?**

Препоръчваме ви да създадете план за преход за уеб базите данни на Access на вашата организация. Администраторите могат да използват [скенера SharePoint на приложенията на Access,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) за да получат наличност на приложенията на Access, които се използват от сайтовете.

Има няколко начина за мигриране на данни от уеб бази данни на Access:

- Импортиране в локална база данни на Access (. ACCDB) или към Excel файл.
- Препоръчваме също да Microsoft PowerApps като алтернативна платформа за създаване на бизнес решения без код за уеб и мобилни устройства.