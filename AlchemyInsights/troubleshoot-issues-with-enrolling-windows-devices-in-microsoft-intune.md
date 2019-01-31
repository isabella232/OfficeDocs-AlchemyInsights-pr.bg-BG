---
title: Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661501"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d7378-102">Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d7378-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d7378-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="d7378-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d7378-104">Някои често срещани съобщения за грешка и разрешаване стъпки:</span><span class="sxs-lookup"><span data-stu-id="d7378-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d7378-p101">**Не може да бъде инсталиран софтуер, 0x80cf4017:** Сертификат вашия акаунт е изтекъл. Повторно изтегляне компютър клиент софтуерен пакет в на Intune административната конзола. Прегледайте документацията за повече информация.</span><span class="sxs-lookup"><span data-stu-id="d7378-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="d7378-108">**Код на грешка 0x801c0003:** Тази грешка може да възникне в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="d7378-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="d7378-p102">Потребителят има повече устройства, записани от лимита за устройството. Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d7378-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="d7378-p103">"Потребителите може да присъедини устройства към лазурните АД" е настроен на "няма". Поставям то към всички или изберете потребители. Прегледайте [документацията](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="d7378-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="d7378-p104">Устройството вече е записан от друг потребител. Ако случаят е такъв, премахнете устройството от Azure Intune конзола или ръчно unenroll устройство преди да опитате отново.</span><span class="sxs-lookup"><span data-stu-id="d7378-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="d7378-p105">Устройството е Windows 10 Начало. Само Windows 10 Pro, образование и предприятието ие може да обединяват Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d7378-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="d7378-118">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="d7378-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d7378-p106">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="d7378-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d7378-121">Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [отстраняване на док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d7378-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="d7378-122">[Научете как да се запишат устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d7378-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

