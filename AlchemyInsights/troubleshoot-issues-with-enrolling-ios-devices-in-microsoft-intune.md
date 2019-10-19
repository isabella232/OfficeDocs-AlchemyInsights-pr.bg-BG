---
title: Отстраняване на проблеми с записване на iOS устройства в Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506870"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Отстраняване на проблеми с записване на iOS устройства в Microsoft InTune

Прегледайте ресурсите, изброени по-долу, за да разрешите вашия проблем сега. 
  
Някои често срещани съобщения за грешки и стъпки за разрешаване:
  
- **Достигнат е капачката на устройството** Потребителят има включени повече устройства от лимита на устройството. Прегледайте тези документи, за да [премахнете дадено устройство](https://docs.microsoft.com/intune/devices-wipe) или да [промените лимита на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Тази услуга не се поддържа. Правила за записване:** Apple Push уведомяване услуга (APNS) трябва да бъде конфигуриран или подновен. Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това. 
    
- **Тип на потребителски лиценз невалидно или потребителско име не е разпознато:** Потребителят трябва да бъде назначен InTune или EMS лиценз. Прегледайте тези документи, за да присвоите лиценз чрез: [център за администриране на Office](https://docs.microsoft.com/intune/licenses-assign) или [Azure портал](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Допълнителни ресурси за разрешаване на проблема ви:
  
1. Използвайте [InTune портал за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностициране и разрешаване на често срещани откази при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Прегледайте тези документи за списък с често срещани грешки, които предотвратяват записването и решенията на всеки: [ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и отстраняване на проблеми с [док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Научете как да записвате устройства с IOS в Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

