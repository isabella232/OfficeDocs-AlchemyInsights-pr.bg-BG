---
title: Работа с iOS VPP приложения Правило ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719946"
---
# <a name="working-with-ios-vpp-applications"></a>Работа с iOS VPP приложения

Прочетете [Как да управлявате iOS приложения, закупени чрез програма за закупуване на том с Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) за да научите за функции, ограничения и стъпки, за да се възползват от програмата apple Том покупка и подкрепата за него в Microsoft Intune.
  
 **Често срещани въпроси:** "Присвоих iOS VPP приложение на моите потребители, но инсталирането не беше успешно."
  
- Това може да се случи, ако един VPP маркер се използва в няколко доставчици на мобилни устройства за управление. VPP маркери от Apple могат да се използват само с един доставчик. Ако сте използвали VPP маркер с няколко доставчика, трябва да качите отново маркера intune.

- Инсталацията може да се провали, ако общият брой инсталации надвишава броя на лицензите. За да видите отчет за употребата на лицензите си, отидете на страницата лицензи за приложения за мобилни **приложения** \> **в Intune.** За да научите как да си възобновете лицензива в употреба, вижте [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
