---
title: Отстраняване на проблеми със записване iOS устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276709"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="cd52e-102">Отстраняване на проблеми със записване iOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cd52e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="cd52e-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="cd52e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="cd52e-104">Някои често срещани съобщения за грешка и разрешаване стъпки:</span><span class="sxs-lookup"><span data-stu-id="cd52e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="cd52e-p101">**Устройството ОСП достига** Потребителят има повече устройства, записани от лимита за устройството. Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/en-us/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="cd52e-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="cd52e-p102">**Тази услуга не се поддържа. Няма правила за записване:** Apple бутам съобщаване служба (APNS) трябва да бъде конфигуриран или подновен. Преглед на [този документ](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) за инструкции как да направите това.</span><span class="sxs-lookup"><span data-stu-id="cd52e-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="cd52e-p103">**Потребител лиценз тип невалиден или потребителско име не се разпознава:** Потребителят трябва да бъде назначен Intune или EMS лиценз. Преглед на тези документи, за да присвоите даден лиценз чрез: [Центъра за администрация на офис](https://docs.microsoft.com/en-us/intune/licenses-assign) или [небесносин портал](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="cd52e-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="cd52e-111">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="cd52e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="cd52e-p104">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="cd52e-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="cd52e-114">Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [отстраняване на док](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="cd52e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="cd52e-115">[Научете как да се запишат iOS устройства в Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="cd52e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

