---
title: Отстраняване на проблеми при записване на устройства с Android в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008067"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на устройства с Android в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.
  
Някои често срещани проблеми и стъпки за разрешаване:
  
 **Грешка "Устройство не е шифровано" Company Portal:** По-новите версии на Android, особено започвайки с v7.0, изискват парола за стартиране, за да се уверите, че устройството ви е напълно шифровано. Често срещаните решения са да разрешите закачите за стартиране или напълно да шифровате устройството. Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.
  
 Устройствата не успяват да се внедлят с услугата Intune или да се показват като **"Нездравослеви" в конзолата за администриране на Intune:** Някои устройства samsung 4.4 и 5.5 може да не се влязат в услугата. Има 3 възможни решения на този проблем:
  
1. Ръчно отворете приложението Intune Company Portal, което автоматично ще инициира синхронизиране на устройството.

2. Актуализирайте устройството до Android 6.0 или по-нова версия.

3. Забраняване на Samsung Smart Manager да управлява Intune Company Portal. Прегледайте [този](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) документ за повече подробности относно тези проблеми и решения.

 **Потребителски лиценз Тип Невалиден** или Потребителско име Не е разпознато **грешка:** Потребителят трябва да бъде назначен лиценз за Intune или EMS. Прегледайте тези документи, за да дадете лиценз чрез: Office център за администриране или портал на Azure.
  
Допълнителни ресурси, които да ви помогнат да решите проблема си:
  
1. Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

2. Прегледайте [този документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които не позволяват записването и разрешаването на всеки от тях.

3. [Научете как да записвате устройства с Android в Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
