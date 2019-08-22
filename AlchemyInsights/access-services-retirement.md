---
title: Достъп до услуги за пенсиониране
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495740"
---
# <a name="access-services-retirement"></a>Достъп до услуги за пенсиониране

Тъй като ние първоначално обявени в MC97576, през март 2017 г. и продължава да комуникират през изминалата година достъп до услуги са се оттегля от Office 365. Следващата фаза в този процес ще бъде премахването на Access уеб бази данни, които използват SharePoint списъци като техните основни данни съхранение.

**Как това влияе ми?**

Започва юни 2019, ние ще спре създаването на нови бази данни на Access в SharePoint Online и затварям голо възвишение служба и всички останали приложения от април 2020.

**Какво трябва да направя, за да се подготвят за тази промяна?**

Препоръчваме ви да създадете план на преход за уеб бази данни Access за вашата организация. Администраторите могат да използват [SharePoint достъп ап скенер](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) да получи опис на достъп до приложения, които използват сайтове.

Има няколко начина за мигриране на данни от Access уеб бази данни:

- Импортиране към местни достъп до база данни (. ACCDB) или към файл на Excel.
- Ние също така препоръчват изследване Microsoft PowerApps като алтернативна платформа за създаване на некодирани бизнес решения за уеб и мобилни устройства.