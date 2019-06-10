---
title: Достъп до услуги за пенсиониране
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769426"
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