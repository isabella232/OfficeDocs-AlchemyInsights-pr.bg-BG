---
title: Отстраняване на проблеми с включването на Android устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655872"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="229af-102">Отстраняване на проблеми с включването на Android устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="229af-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="229af-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="229af-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="229af-104">Някои често срещани проблеми и решителност стъпвам:</span><span class="sxs-lookup"><span data-stu-id="229af-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="229af-p101">**Устройство не шифрова грешка в компанията портал:** По-нови версии на андроид, особено като се започне с v7.0, изискват стартиране парола да се уверите, че устройството ви е изцяло шифрована. Са общи решения за разрешаване на ПИН код за стартиране или напълно шифроване на устройството. Преглед на [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="229af-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="229af-p102">**Устройства не успяват да проверите с услугата на Intune или покажете като "Нездравословното" в административната конзола Intune:** Някои Samsung 4,4 и 5,5 устройства не могат да проверят в услугата. Има 3 възможни решения на този проблем:</span><span class="sxs-lookup"><span data-stu-id="229af-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="229af-110">Ръчно отваряне на Intune компания портал апартамент, който автоматично ще започне синхронизиране на устройството.</span><span class="sxs-lookup"><span data-stu-id="229af-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="229af-111">Актуализиране на устройството за андроид 6.0 или по-висока.</span><span class="sxs-lookup"><span data-stu-id="229af-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="229af-p103">Забраняване на Samsung Smart мениджър от управлението на Intune компания портал. Преглед на [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности по тези въпроси и резолюции.</span><span class="sxs-lookup"><span data-stu-id="229af-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="229af-p104">**Потребителски лиценз тип невалиден** или **потребителско име не се разпознава грешка:** потребителят трябва да бъде присвоен лиценз Intune или EMS. Преглед на тези документи, за да присвоите даден лиценз чрез: офис администратор център или Azure портал.</span><span class="sxs-lookup"><span data-stu-id="229af-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="229af-116">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="229af-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="229af-p105">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="229af-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="229af-119">Преглед на [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък на често срещани грешки, които пречат записване и резолюции на всеки.</span><span class="sxs-lookup"><span data-stu-id="229af-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="229af-120">[Научете как да се запишат на Android устройства в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="229af-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

