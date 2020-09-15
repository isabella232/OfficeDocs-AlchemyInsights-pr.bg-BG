---
title: Пенсиониране в Access Services
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
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698635"
---
# <a name="access-services-retirement"></a>Пенсиониране в Access Services

Както първоначално обявихме в MC97576, през март 2017 и продължихме да комуникираме през изминалите услуги за достъп до години, се оттегляме. Следващият етап на този процес ще бъде премахването на уеб бази данни на Access, които използват списъци на SharePoint като тяхно място за съхранение на данни.

**Как става това?**

Започвайки от юни 2019, ние ще спрем създаването на нови бази данни на Access в SharePoint online и изключете услугата и всички останали приложения от април 2020.

**Какво трябва да направя, за да се подготвя за тази промяна?**

Насърчаваме ви да създадете преходен план за уеб бази данни на Access на вашата организация. Администраторите могат да използват [скенера за приложения на Access на SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , за да получат опис на приложенията на Access, които използват сайтовете.

Има няколко начина за мигриране на данните на уеб базите данни на Access:

- Импортиране в локална база данни на Access (. ACCDB) или към файл на Excel.
- Препоръчваме също да изследвате Microsoft PowerApps като алтернативна платформа, за да създавате бизнес решения без кодове за уеб и мобилни устройства.