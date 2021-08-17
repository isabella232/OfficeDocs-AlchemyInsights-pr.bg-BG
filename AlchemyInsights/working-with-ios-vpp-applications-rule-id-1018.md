---
title: Работа с iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083003"
---
# <a name="working-with-ios-vpp-applications"></a>Работа с VPP приложения на iOS

Прочетете [Как да управлявате приложенията на iOS,](https://docs.microsoft.com/intune/vpp-apps-ios) закупени чрез програма за закупуване на обем с Microsoft Intune, за да научите за функциите, ограниченията и стъпките, за да се възползват от програмата за закупуване на обем на Apple и поддръжката за нея в Microsoft Intune.
  
 **Често срещани проблеми:** "Присвоих VPP приложение на iOS на моите потребители, но инсталирането е неуспешно".
  
- Това може да се случи, ако се използва един VPP маркер за множество доставчици на управление на мобилни устройства. VPP маркери от Apple могат да се използват само с един доставчик. Ако сте използвали VPP маркер с множество доставчици, трябва да качите маркера отново в Intune.

- Инсталирането може също да е неуспешно, ако общият брой инсталации надхвърля броя на лицензите. За да прегледате отчет за използването на вашите лицензи, отидете на страницата Лицензи за приложения на **Intune** \>  Mobile. За да научите как да си възстановят лицензите в употреба, вижте [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
