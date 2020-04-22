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
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="054f0-102">Отстраняване на проблеми при записване на android устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="054f0-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="054f0-103">Прегледайте ресурсите, изброени по-долу, за да разрешите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="054f0-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="054f0-104">Някои често срещани проблеми и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="054f0-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="054f0-105">**Устройство не шифрована грешка в портала на компанията:** По-новите версии на Android, особено като се започне с v7.0, изискват стартова парола, за да се уверите, че устройството ви е напълно шифровано.</span><span class="sxs-lookup"><span data-stu-id="054f0-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="054f0-106">Общите решения са да се даде възможност на стартовия щифт или да се криптира напълно устройството.</span><span class="sxs-lookup"><span data-stu-id="054f0-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="054f0-107">Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="054f0-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="054f0-108">**Устройства не успее да се провери с Intune услуга или се показва като "нездравословни" в intune администратор конзола:** Някои устройства Samsung 4.4 и 5.5 може да не се регистрират в услугата.</span><span class="sxs-lookup"><span data-stu-id="054f0-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="054f0-109">Има 3 възможни решения на този проблем:</span><span class="sxs-lookup"><span data-stu-id="054f0-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="054f0-110">Ръчно отворете приложението Intune Company Portal, което автоматично ще започне синхронизиране на устройство.</span><span class="sxs-lookup"><span data-stu-id="054f0-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="054f0-111">Актуализирайте устройството до Android 6.0 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="054f0-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="054f0-112">Деактивирайте Samsung Smart Manager от управлението на портала на Intune компанията.</span><span class="sxs-lookup"><span data-stu-id="054f0-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="054f0-113">Прегледайте [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности по тези въпроси и решения.</span><span class="sxs-lookup"><span data-stu-id="054f0-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="054f0-114">**Невалиден тип потребителски лиценз** или **потребителско име не е разпознат грешка:** Потребителят трябва да бъде присвоен Intune или EMS лиценз.</span><span class="sxs-lookup"><span data-stu-id="054f0-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="054f0-115">Прегледайте тези документи, за да присвоите лиценз чрез: Център за администриране на Office или Портал на Azure.</span><span class="sxs-lookup"><span data-stu-id="054f0-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="054f0-116">Допълнителни ресурси за разрешаване на проблема:</span><span class="sxs-lookup"><span data-stu-id="054f0-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="054f0-117">Използвайте [Intune портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи грешки при записване.</span><span class="sxs-lookup"><span data-stu-id="054f0-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="054f0-118">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="054f0-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="054f0-119">Прегледайте [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които не позволяват записване и решения за всеки.</span><span class="sxs-lookup"><span data-stu-id="054f0-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="054f0-120">[Научете как да запишете Android устройства в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="054f0-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
