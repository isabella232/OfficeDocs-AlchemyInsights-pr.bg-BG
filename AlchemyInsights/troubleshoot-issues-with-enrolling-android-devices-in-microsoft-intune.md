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
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="fea45-102">Отстраняване на проблеми при записване на устройства с Android в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fea45-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="fea45-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="fea45-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="fea45-104">Някои често срещани проблеми и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="fea45-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="fea45-105">**Грешка "Устройство не е шифровано" в портала на фирмата:** По-новите версии на Android, особено започвайки с v7.0, изискват парола за стартиране, за да се уверите, че устройството ви е напълно шифровано.</span><span class="sxs-lookup"><span data-stu-id="fea45-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="fea45-106">Често срещаните решения са да разрешите закачите за стартиране или напълно да шифровате устройството.</span><span class="sxs-lookup"><span data-stu-id="fea45-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="fea45-107">Прегледайте [този документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="fea45-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="fea45-108">Устройствата не успяват да се внедлят с услугата Intune или да се показват като **"Нездравослеви" в конзолата за администриране на Intune:** Някои устройства samsung 4.4 и 5.5 може да не се влязат в услугата.</span><span class="sxs-lookup"><span data-stu-id="fea45-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="fea45-109">Има 3 възможни решения на този проблем:</span><span class="sxs-lookup"><span data-stu-id="fea45-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="fea45-110">Отворете ръчно приложението Intune Company Portal, което автоматично ще инициира синхронизиране на устройството.</span><span class="sxs-lookup"><span data-stu-id="fea45-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="fea45-111">Актуализирайте устройството до Android 6.0 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="fea45-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="fea45-112">Забраняване на Samsung Smart Manager да управлява портала на компанията Intune.</span><span class="sxs-lookup"><span data-stu-id="fea45-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="fea45-113">Прегледайте [този](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) документ за повече подробности относно тези проблеми и решения.</span><span class="sxs-lookup"><span data-stu-id="fea45-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="fea45-114">**Потребителски лиценз Тип Невалиден** или Потребителско име Не е разпознато **грешка:** Потребителят трябва да бъде назначен лиценз за Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="fea45-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="fea45-115">Прегледайте тези документи, за да дадете лиценз чрез: Център за администриране на Office или портал на Azure.</span><span class="sxs-lookup"><span data-stu-id="fea45-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="fea45-116">Допълнителни ресурси, които да ви помогнат да решите проблема си:</span><span class="sxs-lookup"><span data-stu-id="fea45-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="fea45-117">Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване.</span><span class="sxs-lookup"><span data-stu-id="fea45-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="fea45-118">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="fea45-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="fea45-119">Прегледайте [този документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) за списък с често срещани грешки, които не позволяват записването и разрешаването на всеки от тях.</span><span class="sxs-lookup"><span data-stu-id="fea45-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="fea45-120">[Научете как да записвате устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="fea45-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
