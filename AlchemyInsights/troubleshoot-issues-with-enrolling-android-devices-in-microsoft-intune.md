---
title: Отстраняване на проблеми с включването на Android устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420581"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Отстраняване на проблеми с включването на Android устройства в Microsoft Intune

Преглед на ресурси, изброени по-долу да решим вашия проблем сега.
  
Някои често срещани проблеми и решителност стъпвам:
  
 **Устройство не шифрова грешка в компанията портал:** По-нови версии на андроид, особено като се започне с v7.0, изискват стартиране парола да се уверите, че устройството ви е изцяло шифрована. Са общи решения за разрешаване на ПИН код за стартиране или напълно шифроване на устройството. Преглед на [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация. 
  
 **Устройства не успяват да проверите с услугата на Intune или покажете като "Нездравословното" в административната конзола Intune:** Някои Samsung 4,4 и 5,5 устройства не могат да проверят в услугата. Има 3 възможни решения на този проблем: 
  
1. Ръчно отваряне на Intune компания портал апартамент, който автоматично ще започне синхронизиране на устройството.
    
2. Актуализиране на устройството за андроид 6.0 или по-висока.
    
3. Забраняване на Samsung Smart мениджър от управлението на Intune компания портал. Преглед на [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности по тези въпроси и резолюции. 
    
 **Потребителски лиценз тип невалиден** или **потребителско име не се разпознава грешка:** потребителят трябва да бъде присвоен лиценз Intune или EMS. Преглед на тези документи, за да присвоите даден лиценз чрез: офис администратор център или Azure портал. 
  
Допълнителни ресурси за разрешаване на вашия проблем:
  
1. Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Преглед на [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък на често срещани грешки, които пречат записване и резолюции на всеки. 
    
3. [Научете как да се запишат на Android устройства в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

