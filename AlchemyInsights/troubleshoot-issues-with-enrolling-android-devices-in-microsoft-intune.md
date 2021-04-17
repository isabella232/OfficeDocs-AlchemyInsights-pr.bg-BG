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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830931"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записване на устройства с Android в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.
  
Някои често срещани проблеми и стъпки за разрешаване:
  
 **Грешка "Устройство не е шифровано" в портала на фирмата:** По-новите версии на Android, особено започвайки с v7.0, изискват парола за стартиране, за да се уверите, че устройството ви е напълно шифровано. Често срещаните решения са да разрешите закачите за стартиране или напълно да шифровате устройството. Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.
  
 Устройствата не успяват да се внедлят с услугата Intune или да се показват като **"Нездравослеви" в конзолата за администриране на Intune:** Някои устройства samsung 4.4 и 5.5 може да не се влязат в услугата. Има 3 възможни решения на този проблем:
  
1. Отворете ръчно приложението Intune Company Portal, което автоматично ще инициира синхронизиране на устройството.

2. Актуализирайте устройството до Android 6.0 или по-нова версия.

3. Забраняване на Samsung Smart Manager да управлява портала на компанията Intune. Прегледайте [този](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) документ за повече подробности относно тези проблеми и решения.

 **Потребителски лиценз Тип Невалиден** или Потребителско име Не е разпознато **грешка:** Потребителят трябва да бъде назначен лиценз за Intune или EMS. Прегледайте тези документи, за да дадете лиценз чрез: Център за администриране на Office или портал на Azure.
  
Допълнителни ресурси, които да ви помогнат да решите проблема си:
  
1. Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

2. Прегледайте [този документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които не позволяват записването и разрешаването на всеки от тях.

3. [Научете как да записвате устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
