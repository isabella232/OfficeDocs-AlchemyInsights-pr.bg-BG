---
title: Отстраняване на проблеми при записването на устройства с Windows в Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708879"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d991f-102">Отстраняване на проблеми при записването на устройства с Windows в Microsoft</span><span class="sxs-lookup"><span data-stu-id="d991f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d991f-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="d991f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d991f-104">Някои често срещани съобщения за грешка и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="d991f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d991f-105">**Софтуерът не може да се инсталира, 0x80cf4017:** Вашият сертификат за акаунт е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="d991f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d991f-106">Изтеглете отново пакета за софтуерни клиенти на PC в конзолата за администриране на администратора.</span><span class="sxs-lookup"><span data-stu-id="d991f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d991f-107">Прегледайте тази документация за повече информация.</span><span class="sxs-lookup"><span data-stu-id="d991f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d991f-108">**Код на грешка 0x801c0003:** Грешката може да възникне в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="d991f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d991f-109">Потребителят има повече устройства, записани от лимита на устройството.</span><span class="sxs-lookup"><span data-stu-id="d991f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d991f-110">Прегледайте тези документи, за да [премахнете устройство](https://docs.microsoft.com/intune/devices-wipe) или да [промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d991f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d991f-111">"Потребителите могат да се присъединят към устройства в Azure AD" е зададено на "няма".</span><span class="sxs-lookup"><span data-stu-id="d991f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d991f-112">Настройте го на всички или изберете потребители.</span><span class="sxs-lookup"><span data-stu-id="d991f-112">Set it to all or select users.</span></span> <span data-ttu-id="d991f-113">Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="d991f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d991f-114">Устройството вече е записано от друг потребител.</span><span class="sxs-lookup"><span data-stu-id="d991f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d991f-115">Ако това е така, премахнете устройството от конзолата за настройване на Azure или ръчно отменете устройството, преди да опитате отново.</span><span class="sxs-lookup"><span data-stu-id="d991f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d991f-116">Устройството е Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="d991f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d991f-117">Само Windows 10 Pro, Education и Enterprise МСА могат да се присъединят към Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d991f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d991f-118">Допълнителни ресурси, които да ви помогнат да отстраните проблема:</span><span class="sxs-lookup"><span data-stu-id="d991f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d991f-119">Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания.</span><span class="sxs-lookup"><span data-stu-id="d991f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d991f-120">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="d991f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d991f-121">Прегледайте тези документи за списък с често срещани грешки, които пречат на записването и резолюциите във всеки от тях: [ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [отстраняване на неизправности](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d991f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d991f-122">[Научете как да записвате устройства с Windows в Microsoft](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d991f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
