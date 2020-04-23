---
title: Отстраняване на проблеми при записване на IOS устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736147"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на IOS устройства в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да разрешите проблема си сега. 
  
Някои често срещани съобщения за грешки и стъпки за разрешаване:
  
- **Достигната е капачката на устройството** Потребителят има повече устройства, записани от ограничението на устройството. Прегледайте тези документи, за да [премахнете устройство](https://docs.microsoft.com/intune/devices-wipe) или [да промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Тази услуга не се поддържа. Политика за записване:** Apple push Notification Service (APNS) трябва да бъде конфигуриран или подновен. Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това. 
    
- **Невалиден тип потребителски лиценз или нееразен потребител:** Потребителят трябва да получи лиценз intune или EMS. Прегледайте тези документи, за да присвоите лиценз чрез: [Център за администрация](https://docs.microsoft.com/intune/licenses-assign) на Office или Портал на [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Допълнителни ресурси за разрешаване на проблема:
  
1. Използвайте [Intune портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Прегледайте тези документи за списък с често срещани грешки, които предотвратяват записването и решенията за всеки: [Ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и отстраняване на неизправности [док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Научете как да запишете IOS устройства в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

