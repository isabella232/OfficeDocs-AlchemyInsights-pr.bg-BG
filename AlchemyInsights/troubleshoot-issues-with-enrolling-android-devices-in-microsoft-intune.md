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
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="facab-102">Отстраняване на проблеми при записването на устройства с Android в Microsoft</span><span class="sxs-lookup"><span data-stu-id="facab-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="facab-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="facab-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="facab-104">Някои често срещани проблеми и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="facab-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="facab-105">**Устройството не е шифровано грешка във фирмения портал:** По-новите версии на Android, по-специално започвайки с v 7.0, изискват парола при стартиране, за да се уверите, че вашето устройство е напълно шифровано.</span><span class="sxs-lookup"><span data-stu-id="facab-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="facab-106">Общи решения са за разрешаване на ПИН код за стартиране или за пълно шифроване на устройството.</span><span class="sxs-lookup"><span data-stu-id="facab-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="facab-107">Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="facab-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="facab-108">**Устройства не успяват да се вкарат при настройването на услугата или да се показват като "нездравословен" в конзолата за администриране на администратора:** Някои устройства Samsung 4,4 и 5,5 може да не проверяват услугата.</span><span class="sxs-lookup"><span data-stu-id="facab-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="facab-109">Има три възможни решения за този проблем:</span><span class="sxs-lookup"><span data-stu-id="facab-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="facab-110">Ръчно отваряте приложението за въвеждане на фирмения портал, което автоматично ще инициира синхронизиране на устройството.</span><span class="sxs-lookup"><span data-stu-id="facab-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="facab-111">Актуализирайте устройството с Android 6,0 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="facab-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="facab-112">Забранете Samsung Smart Manager от управлението на портала за фирми за настройване.</span><span class="sxs-lookup"><span data-stu-id="facab-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="facab-113">Прегледайте [този документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) за повече подробности относно тези проблеми и резолюции.</span><span class="sxs-lookup"><span data-stu-id="facab-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="facab-114">**Невалиден тип потребителски лиценз** или **потребителско име не е разпозната грешка:** потребителят трябва да получи лиценз за настройване или EMS.</span><span class="sxs-lookup"><span data-stu-id="facab-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="facab-115">Прегледайте тези документи, за да дадете лиценз чрез: център за администриране на Office или портал на Azure.</span><span class="sxs-lookup"><span data-stu-id="facab-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="facab-116">Допълнителни ресурси, които да ви помогнат да отстраните проблема:</span><span class="sxs-lookup"><span data-stu-id="facab-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="facab-117">Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания.</span><span class="sxs-lookup"><span data-stu-id="facab-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="facab-118">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="facab-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="facab-119">Прегледайте [този документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които забраняват записването и резолюциите във всеки от тях.</span><span class="sxs-lookup"><span data-stu-id="facab-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="facab-120">[Научете как да запишете устройства с Android в Microsoft](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="facab-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
