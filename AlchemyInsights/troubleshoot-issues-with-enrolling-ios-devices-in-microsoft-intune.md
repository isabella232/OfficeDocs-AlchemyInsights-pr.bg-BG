---
title: Отстраняване на проблеми при записване на устройства с iOS в Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708951"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на устройства с iOS в Microsoft

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега. 
  
Някои често срещани съобщения за грешка и стъпки за разрешаване:
  
- **Достигната е капачка на устройството** Потребителят има повече устройства, записани от лимита на устройството. Прегледайте тези документи, за да [премахнете устройство](https://docs.microsoft.com/intune/devices-wipe) или да [промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Тази услуга не се поддържа. Без правила за записване:** услуга за насочени известия за Apple (APN) трябва да бъде конфигурирана или подновена. Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да го направите. 
    
- **Тип на потребителски лиценз за невалидно или потребителско име не е разпознат:** На потребителя трябва да бъде назначен лиценз за настройване или EMS. Прегледайте тези документи, за да дадете лиценз чрез: [център за администриране на Office](https://docs.microsoft.com/intune/licenses-assign) или портал на [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Допълнителни ресурси, които да ви помогнат да отстраните проблема:
  
1. Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Прегледайте тези документи за списък с често срещани грешки, които пречат на записването и резолюциите във всеки от тях: [ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [отстраняване на неизправности](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Научете как да регистрирате устройства с IOS в Microsoft](https://docs.microsoft.com/intune/ios-enroll).
    

