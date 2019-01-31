---
title: Отстраняване на проблеми със записване iOS устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658428"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Отстраняване на проблеми със записване iOS устройства в Microsoft Intune

Преглед на ресурси, изброени по-долу да решим вашия проблем сега. 
  
Някои често срещани съобщения за грешка и разрешаване стъпки:
  
- **Устройството ОСП достига** Потребителят има повече устройства, записани от лимита за устройството. Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Тази услуга не се поддържа. Няма правила за записване:** Apple бутам съобщаване служба (APNS) трябва да бъде конфигуриран или подновен. Преглед на [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това. 
    
- **Потребител лиценз тип невалиден или потребителско име не се разпознава:** Потребителят трябва да бъде назначен Intune или EMS лиценз. Преглед на тези документи, за да присвоите даден лиценз чрез: [Центъра за администрация на офис](https://docs.microsoft.com/intune/licenses-assign) или [небесносин портал](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Допълнителни ресурси за разрешаване на вашия проблем:
  
1. Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [отстраняване на док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Научете как да се запишат iOS устройства в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

