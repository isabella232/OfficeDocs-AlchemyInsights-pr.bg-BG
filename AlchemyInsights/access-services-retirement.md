---
title: Достъп до услуги за пенсиониране
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747773"
---
# <a name="access-services-retirement"></a>Достъп до услуги за пенсиониране

Както първоначално обяви през MC97576., през март 2017, и продължи да комуникира през изминалата година услугите за достъп се пенсионираха от Office 365. Следващата фаза в този процес ще бъде премахването на Access Web бази данни, които използват списъците на SharePoint като основни данни за съхранение.

**Как се отразява това на мен?**

От юни 2019, ние ще спрем създаването на нови бази данни на Access в SharePoint online и изключете услугата и всички останали приложения до април 2020.

**Какво трябва да направя, за да се подготвя за тази промяна?**

Насърчаваме ви да създадете план за преход за уеб базите данни за Access на вашата организация. Администраторите могат да използват [сканиране на приложението на SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , за да получите списък на приложенията на Access, които сайтовете използват.

Има няколко начина за мигриране на данните за уеб бази данни на Access:

- Импортиране в локална база данни на Access (. ACCDB) или към файл на Excel.
- Също така препоръчваме да разгледате Microsoft PowerApps като алтернативна платформа, за да създадете некодови бизнес решения за уеб и мобилни устройства.