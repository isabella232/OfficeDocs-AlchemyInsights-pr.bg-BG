---
title: Отстраняване на проблеми при записване на устройства с iOS в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823452"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="7bf66-102">Отстраняване на проблеми при записване на устройства с iOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7bf66-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="7bf66-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="7bf66-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="7bf66-104">Някои често срещани съобщения за грешки и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="7bf66-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="7bf66-105">**Достигната е капачката на устройството** Потребителят има повече записани устройства от ограничението на устройството.</span><span class="sxs-lookup"><span data-stu-id="7bf66-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7bf66-106">Прегледайте тези [документи, за да премахнете устройство или](https://docs.microsoft.com/intune/devices-wipe) да промените [ограничението за устройството.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7bf66-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="7bf66-107">**Тази услуга не се поддържа. Без правила за записване:** Услугата за push notification (APNS) на Apple трябва да бъде конфигурирана или подновена.</span><span class="sxs-lookup"><span data-stu-id="7bf66-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="7bf66-108">Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това.</span><span class="sxs-lookup"><span data-stu-id="7bf66-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="7bf66-109">**Тип на потребителски лиценз Невалиден или Потребителско име не е разпознато:** Потребителят трябва да бъде назначен лиценз за Intune или EMS.</span><span class="sxs-lookup"><span data-stu-id="7bf66-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7bf66-110">Прегледайте тези документи, за да дадете лиценз чрез: [Център за администриране на Office](https://docs.microsoft.com/intune/licenses-assign) или портал на [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="7bf66-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="7bf66-111">Допълнителни ресурси, които да ви помогнат да решите проблема си:</span><span class="sxs-lookup"><span data-stu-id="7bf66-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7bf66-112">Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване.</span><span class="sxs-lookup"><span data-stu-id="7bf66-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7bf66-113">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="7bf66-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7bf66-114">Прегледайте тези документи за списък с често срещани грешки, които не позволяват записването и разделителната способност на всеки: Ръководство за отстраняване на [неизправности и](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) документ за отстраняване [на неизправности.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7bf66-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="7bf66-115">[Научете как да записвате устройства с iOS в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="7bf66-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

