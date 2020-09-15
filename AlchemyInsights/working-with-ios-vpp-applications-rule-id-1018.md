---
title: Работа с ИД на правило за приложения на iOS с 1018
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688935"
---
# <a name="working-with-ios-vpp-applications"></a>Работа с приложения на iOS VPP

Прочетете [как да управлявате приложенията на IOS, закупени чрез програма за закупуване на обем, с Microsoft](https://docs.microsoft.com/intune/vpp-apps-ios) за да научите за функциите, ограниченията и стъпките, за да се възползвате от програмата за закупуване на томове на Apple и поддръжката за нея в Microsoft.
  
 **Често срещани проблеми:** "Дадох на моите потребители приложение на iOS VPP, но инсталирането е неуспешно."
  
- Това може да се случи, ако се използва единичен маркер за VPP точка в множество доставчици на управление на мобилни устройства. VPP маркери от Apple могат да се използват само с един доставчик. Ако сте използвали маркер на VPP точка с множество доставчици, трябва отново да качите маркера, за да го настроите.

- Инсталацията може да се провали и ако общият брой на инсталациите надвишава броя на лицензите. За да видите отчет за използването за вашите лицензи, отидете на страницата за лицензи за приложения на **мобилното** \> **приложение** . За да научите как да поискате да се възстановят лицензи в употреба, вижте [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
