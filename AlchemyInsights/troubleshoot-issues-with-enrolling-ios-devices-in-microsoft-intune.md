---
title: Отстраняване на проблеми при записване на устройства с iOS в Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669237"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="474fc-102">Отстраняване на проблеми при записване на устройства с iOS в Microsoft</span><span class="sxs-lookup"><span data-stu-id="474fc-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="474fc-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="474fc-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="474fc-104">Някои често срещани съобщения за грешка и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="474fc-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="474fc-105">**Достигната е капачка на устройството** Потребителят има повече устройства, записани от лимита на устройството.</span><span class="sxs-lookup"><span data-stu-id="474fc-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="474fc-106">Прегледайте тези документи, за да [премахнете устройство](https://docs.microsoft.com/intune/devices-wipe) или да [промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="474fc-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="474fc-107">**Тази услуга не се поддържа. Без правила за записване:** услуга за насочени известия за Apple (APN) трябва да бъде конфигурирана или подновена.</span><span class="sxs-lookup"><span data-stu-id="474fc-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="474fc-108">Прегледайте [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да го направите.</span><span class="sxs-lookup"><span data-stu-id="474fc-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="474fc-109">**Тип на потребителски лиценз за невалидно или потребителско име не е разпознат:** На потребителя трябва да бъде назначен лиценз за настройване или EMS.</span><span class="sxs-lookup"><span data-stu-id="474fc-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="474fc-110">Прегледайте тези документи, за да дадете лиценз чрез: [център за администриране на Office](https://docs.microsoft.com/intune/licenses-assign) или портал на [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="474fc-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="474fc-111">Допълнителни ресурси, които да ви помогнат да отстраните проблема:</span><span class="sxs-lookup"><span data-stu-id="474fc-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="474fc-112">Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания.</span><span class="sxs-lookup"><span data-stu-id="474fc-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="474fc-113">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="474fc-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="474fc-114">Прегледайте тези документи за списък с често срещани грешки, които пречат на записването и резолюциите във всеки от тях: [ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [отстраняване на неизправности](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="474fc-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="474fc-115">[Научете как да регистрирате устройства с IOS в Microsoft](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="474fc-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

