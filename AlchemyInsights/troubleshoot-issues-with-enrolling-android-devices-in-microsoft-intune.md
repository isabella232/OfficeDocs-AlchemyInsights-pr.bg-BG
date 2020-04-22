---
title: Отстраняване на проблеми при записване на android устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759609"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на android устройства в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да разрешите проблема си сега.
  
Някои често срещани проблеми и стъпки за разрешаване:
  
 **Устройство не шифрована грешка в портала на компанията:** По-новите версии на Android, особено като се започне с v7.0, изискват стартова парола, за да се уверите, че устройството ви е напълно шифровано. Общите решения са да се даде възможност на стартовия щифт или да се криптира напълно устройството. Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.
  
 **Устройства не успее да се провери с Intune услуга или се показва като "нездравословни" в intune администратор конзола:** Някои устройства Samsung 4.4 и 5.5 може да не се регистрират в услугата. Има 3 възможни решения на този проблем:
  
1. Ръчно отворете приложението Intune Company Portal, което автоматично ще започне синхронизиране на устройство.

2. Актуализирайте устройството до Android 6.0 или по-нова версия.

3. Деактивирайте Samsung Smart Manager от управлението на портала на Intune компанията. Прегледайте [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности по тези въпроси и решения.

 **Невалиден тип потребителски лиценз** или **потребителско име не е разпознат грешка:** Потребителят трябва да бъде присвоен Intune или EMS лиценз. Прегледайте тези документи, за да присвоите лиценз чрез: Център за администриране на Office или Портал на Azure.
  
Допълнителни ресурси за разрешаване на проблема:
  
1. Използвайте [Intune портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

2. Прегледайте [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които не позволяват записване и решения за всеки.

3. [Научете как да запишете Android устройства в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
