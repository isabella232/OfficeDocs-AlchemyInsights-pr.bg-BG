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
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500060"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="72439-102">Отстраняване на проблеми с включването на Android устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="72439-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="72439-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="72439-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="72439-104">Някои често срещани проблеми и решителност стъпвам:</span><span class="sxs-lookup"><span data-stu-id="72439-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="72439-105">**Устройство не шифрова грешка в компанията портал:** По-нови версии на андроид, особено като се започне с v7.0, изискват стартиране парола да се уверите, че устройството ви е изцяло шифрована.</span><span class="sxs-lookup"><span data-stu-id="72439-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="72439-106">Са общи решения за разрешаване на ПИН код за стартиране или напълно шифроване на устройството.</span><span class="sxs-lookup"><span data-stu-id="72439-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="72439-107">Преглед на [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="72439-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="72439-108">**Устройства не успяват да проверите с услугата на Intune или покажете като "Нездравословното" в административната конзола Intune:** Някои Samsung 4,4 и 5,5 устройства не могат да проверят в услугата.</span><span class="sxs-lookup"><span data-stu-id="72439-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="72439-109">Има 3 възможни решения на този проблем:</span><span class="sxs-lookup"><span data-stu-id="72439-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="72439-110">Ръчно отваряне на Intune компания портал апартамент, който автоматично ще започне синхронизиране на устройството.</span><span class="sxs-lookup"><span data-stu-id="72439-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="72439-111">Актуализиране на устройството за андроид 6.0 или по-висока.</span><span class="sxs-lookup"><span data-stu-id="72439-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="72439-112">Забраняване на Samsung Smart мениджър от управлението на Intune компания портал.</span><span class="sxs-lookup"><span data-stu-id="72439-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="72439-113">Преглед на [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности по тези въпроси и резолюции.</span><span class="sxs-lookup"><span data-stu-id="72439-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="72439-114">**Потребителски лиценз тип невалиден** или **потребителско име не се разпознава грешка:** потребителят трябва да бъде присвоен лиценз Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="72439-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="72439-115">Преглед на тези документи, за да присвоите даден лиценз чрез: офис администратор център или Azure портал.</span><span class="sxs-lookup"><span data-stu-id="72439-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="72439-116">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="72439-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="72439-117">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности.</span><span class="sxs-lookup"><span data-stu-id="72439-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="72439-118">Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="72439-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="72439-119">Преглед на [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък на често срещани грешки, които пречат записване и резолюции на всеки.</span><span class="sxs-lookup"><span data-stu-id="72439-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="72439-120">[Научете как да се запишат на Android устройства в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="72439-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
