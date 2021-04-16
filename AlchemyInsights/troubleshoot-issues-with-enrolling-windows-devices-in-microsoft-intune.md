---
title: Отстраняване на проблеми при записване на устройства с Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808960"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="43a41-102">Отстраняване на проблеми при записване на устройства с Windows в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="43a41-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="43a41-103">Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="43a41-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="43a41-104">Някои често срещани съобщения за грешки и стъпки за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="43a41-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="43a41-105">**Софтуерът не може да бъде инсталиран, 0x80cf4017:** Срокът на вашия сертификат за акаунт е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="43a41-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="43a41-106">Изтеглете отново софтуерния пакет за pc Client в конзолата за администриране на Intune.</span><span class="sxs-lookup"><span data-stu-id="43a41-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="43a41-107">Прегледайте тази документация за повече информация.</span><span class="sxs-lookup"><span data-stu-id="43a41-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="43a41-108">**Код на грешка 0x801c0003:** Грешката може да възникне в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="43a41-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="43a41-109">Потребителят има повече записани устройства от ограничението на устройството.</span><span class="sxs-lookup"><span data-stu-id="43a41-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="43a41-110">Прегледайте тези [документи, за да премахнете устройство или](https://docs.microsoft.com/intune/devices-wipe) да промените [ограничението за устройството.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="43a41-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="43a41-111">"Потребителите могат да се присъединяват към устройства към Azure AD" е зададено на "няма".</span><span class="sxs-lookup"><span data-stu-id="43a41-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="43a41-112">Задайте го на всички или изберете потребители.</span><span class="sxs-lookup"><span data-stu-id="43a41-112">Set it to all or select users.</span></span> <span data-ttu-id="43a41-113">Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="43a41-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="43a41-114">Устройството вече е записано от друг потребител.</span><span class="sxs-lookup"><span data-stu-id="43a41-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="43a41-115">Ако случаят е такъв, премахнете устройството от конзолата Azure Intune или ръчно го премахнете, преди да опитате отново.</span><span class="sxs-lookup"><span data-stu-id="43a41-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="43a41-116">Устройството е Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="43a41-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="43a41-117">Само windows 10 Pro, Education и Enterprise SKUs могат да се присъединят към Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="43a41-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="43a41-118">Допълнителни ресурси, които да ви помогнат да решите проблема си:</span><span class="sxs-lookup"><span data-stu-id="43a41-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="43a41-119">Използвайте [Портала за отстраняване на неизправности в Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за да диагностицирате и отстраните често срещани грешки при записване.</span><span class="sxs-lookup"><span data-stu-id="43a41-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="43a41-120">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="43a41-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="43a41-121">Прегледайте тези документи за списък с често срещани грешки, които не позволяват записването и разделителната способност на всеки: Ръководство за отстраняване на [неизправности и](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) документ за отстраняване [на неизправности.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="43a41-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="43a41-122">[Научете как да записвате устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="43a41-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
