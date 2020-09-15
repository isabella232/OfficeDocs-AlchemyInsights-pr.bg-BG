---
title: Отстраняване на проблеми при записването на устройства с Android в Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689943"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записването на устройства с Android в Microsoft

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.
  
Някои често срещани проблеми и стъпки за разрешаване:
  
 **Устройството не е шифровано грешка във фирмения портал:** По-новите версии на Android, по-специално започвайки с v 7.0, изискват парола при стартиране, за да се уверите, че вашето устройство е напълно шифровано. Общи решения са за разрешаване на ПИН код за стартиране или за пълно шифроване на устройството. Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.
  
 **Устройства не успяват да се вкарат при настройването на услугата или да се показват като "нездравословен" в конзолата за администриране на администратора:** Някои устройства Samsung 4,4 и 5,5 може да не проверяват услугата. Има три възможни решения за този проблем:
  
1. Ръчно отваряте приложението за въвеждане на фирмения портал, което автоматично ще инициира синхронизиране на устройството.

2. Актуализирайте устройството с Android 6,0 или по-нова версия.

3. Забранете Samsung Smart Manager от управлението на портала за фирми за настройване. Прегледайте [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности относно тези проблеми и резолюции.

 **Невалиден тип потребителски лиценз** или **потребителско име не е разпозната грешка:** потребителят трябва да получи лиценз за настройване или EMS. Прегледайте тези документи, за да дадете лиценз чрез: център за администриране на Office или портал на Azure.
  
Допълнителни ресурси, които да ви помогнат да отстраните проблема:
  
1. Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

2. Прегледайте [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които забраняват записването и резолюциите във всеки от тях.

3. [Научете как да запишете устройства с Android в Microsoft](https://docs.microsoft.com/intune/android-enroll).
