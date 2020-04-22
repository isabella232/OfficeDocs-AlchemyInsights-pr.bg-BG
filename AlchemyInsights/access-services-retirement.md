---
title: Пенсиониране на услугите за достъп
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687247"
---
# <a name="access-services-retirement"></a>Пенсиониране на услугите за достъп

Както първоначално обявихме в MC97576, през март 2017 г. и продължида комуникира през изминалата година Услугите за достъп се пенсионират. Следващата фаза в този процес ще бъде премахването на уеб бази данни на Access, които използват списъци на SharePoint като тяхна основна съхранение на данни.

**Как се отразява това на мен?**

От юни 2019, ние ще спре създаването на нови бази данни на Access в SharePoint Online и изключване на услугата и всички останали приложения до април 2020.

**Какво трябва да направя, за да се подготвя за тази промяна?**

Препоръчваме ви да създадете план за преход за уеб базите данни на вашата организация. Администраторите могат да използват скенера на [приложението SharePoint Access,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) за да получите списък на приложенията на Access, които се използват от сайтовете.

Има няколко начина за мигриране на данни за уеб бази данни за Access:

- Импортиране в локална база данни на Access (. accdb) или към файл в Excel.
- Препоръчваме също да проучите Microsoft PowerApps като алтернативна платформа за създаване на бизнес решения без код за уеб и мобилни устройства.