---
title: Отстраняване на проблеми при записване на устройства с Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808960"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на устройства с Windows в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.
  
Някои често срещани съобщения за грешки и стъпки за разрешаване:
  
 **Софтуерът не може да бъде инсталиран, 0x80cf4017:** Срокът на вашия сертификат за акаунт е изтекъл. Изтеглете отново софтуерния пакет за pc Client в конзолата за администриране на Intune. Прегледайте тази документация за повече информация.
  
 **Код на грешка 0x801c0003:** Грешката може да възникне в следните сценарии:
  
-  Потребителят има повече записани устройства от ограничението на устройството. Прегледайте тези [документи, за да премахнете устройство или](https://docs.microsoft.com/intune/devices-wipe) да промените [ограничението за устройството.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Потребителите могат да се присъединяват към устройства към Azure AD" е зададено на "няма". Задайте го на всички или изберете потребители. Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.

-  Устройството вече е записано от друг потребител. Ако случаят е такъв, премахнете устройството от конзолата Azure Intune или ръчно го премахнете, преди да опитате отново.

-  Устройството е Windows 10 Home. Само windows 10 Pro, Education и Enterprise SKUs могат да се присъединят към Azure Active Directory.

Допълнителни ресурси, които да ви помогнат да решите проблема си:
  
-  Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

-  Прегледайте тези документи за списък с често срещани грешки, които не позволяват записването и разделителната способност на всеки: Ръководство за отстраняване на [неизправности и](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) документ за отстраняване [на неизправности.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Научете как да записвате устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
