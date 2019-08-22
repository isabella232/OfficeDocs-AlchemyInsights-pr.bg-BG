---
title: Отстраняване на проблеми със записване iOS устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506870"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9ad71-102">Отстраняване на проблеми със записване iOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9ad71-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9ad71-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="9ad71-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9ad71-104">Някои често срещани съобщения за грешка и разрешаване стъпки:</span><span class="sxs-lookup"><span data-stu-id="9ad71-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9ad71-105">**Устройството ОСП достига** Потребителят има повече устройства, записани от лимита за устройството.</span><span class="sxs-lookup"><span data-stu-id="9ad71-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9ad71-106">Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9ad71-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9ad71-107">**Тази услуга не се поддържа. Няма правила за записване:** Apple бутам съобщаване служба (APNS) трябва да бъде конфигуриран или подновен.</span><span class="sxs-lookup"><span data-stu-id="9ad71-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="9ad71-108">Преглед на [този документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) за инструкции как да направите това.</span><span class="sxs-lookup"><span data-stu-id="9ad71-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9ad71-109">**Потребител лиценз тип невалиден или потребителско име не се разпознава:** Потребителят трябва да бъде назначен Intune или EMS лиценз.</span><span class="sxs-lookup"><span data-stu-id="9ad71-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9ad71-110">Преглед на тези документи, за да присвоите даден лиценз чрез: [Центъра за администрация на офис](https://docs.microsoft.com/intune/licenses-assign) или [небесносин портал](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="9ad71-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9ad71-111">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="9ad71-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9ad71-112">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности.</span><span class="sxs-lookup"><span data-stu-id="9ad71-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9ad71-113">Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="9ad71-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9ad71-114">Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) и [отстраняване на док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9ad71-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9ad71-115">[Научете как да се запишат iOS устройства в Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="9ad71-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

