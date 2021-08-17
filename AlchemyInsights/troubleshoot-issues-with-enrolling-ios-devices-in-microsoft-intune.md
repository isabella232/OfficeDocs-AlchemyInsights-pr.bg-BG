---
title: Отстраняване на проблеми при записване на устройства с iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047965"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на устройства с iOS в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега. 
  
Някои често срещани съобщения за грешки и стъпки за разрешаване:
  
- **Достигната е капачката на устройството** Потребителят има повече записани устройства от ограничението на устройството. Прегледайте тези [документи, за да премахнете устройство или](https://docs.microsoft.com/intune/devices-wipe) да промените [ограничението за устройството.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Тази услуга не се поддържа. Без правила за записване:** Услугата за push notification (APNS) на Apple трябва да бъде конфигурирана или подновена. Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това. 
    
- **Тип на потребителски лиценз Невалиден или Потребителско име не е разпознато:** Потребителят трябва да бъде назначен лиценз за Intune или EMS. Прегледайте тези документи, за да дадете лиценз чрез: [Office център за администриране](https://docs.microsoft.com/intune/licenses-assign) или портал на [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Допълнителни ресурси, които да ви помогнат да решите проблема си:
  
1. Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Прегледайте тези документи за списък с често срещани грешки, които не позволяват записването и разделителната способност на всеки: Ръководство за отстраняване на [неизправности и](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) документ за отстраняване [на неизправности.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Научете как да записвате устройства с iOS в Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

