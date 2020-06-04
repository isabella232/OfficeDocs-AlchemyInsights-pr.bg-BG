---
title: Отстраняване на проблеми със записване на устройства с Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665821"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="77c9d-102">Отстраняване на проблеми със записване на устройства с Windows в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="77c9d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="77c9d-103">Прегледайте ресурсите, изброени по-долу, за да разрешите проблема си сега.</span><span class="sxs-lookup"><span data-stu-id="77c9d-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="77c9d-104">Някои често срещани съобщения за грешки и стъпки за разрешаване на проблема:</span><span class="sxs-lookup"><span data-stu-id="77c9d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="77c9d-105">**Софтуерът не може да бъде инсталиран, 0x80cf4017:** Вашият сертификат за акаунт е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="77c9d-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="77c9d-106">Изтеглете отново клиентския пакет за PC в Intune Admin Console.</span><span class="sxs-lookup"><span data-stu-id="77c9d-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="77c9d-107">Прегледайте тази документация за повече информация.</span><span class="sxs-lookup"><span data-stu-id="77c9d-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="77c9d-108">**Код на грешка 0x801c0003:** Грешка може да възникне в следните ситуации:</span><span class="sxs-lookup"><span data-stu-id="77c9d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="77c9d-109">Потребителят има повече включени устройства от ограничението на устройството.</span><span class="sxs-lookup"><span data-stu-id="77c9d-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="77c9d-110">Прегледайте тези [документи, за](https://docs.microsoft.com/intune/devices-wipe) да премахнете устройство или [да промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="77c9d-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="77c9d-111">"Потребителите могат да се присъедини устройства Azure AD" е зададена на "няма".</span><span class="sxs-lookup"><span data-stu-id="77c9d-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="77c9d-112">Задайте го на всички или изберете потребители.</span><span class="sxs-lookup"><span data-stu-id="77c9d-112">Set it to all or select users.</span></span> <span data-ttu-id="77c9d-113">Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="77c9d-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="77c9d-114">Устройството вече е записано от друг потребител.</span><span class="sxs-lookup"><span data-stu-id="77c9d-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="77c9d-115">Ако случаят е такъв, премахнете устройството от Azure Intune конзолата или ръчно откройте устройството, преди да опитате отново.</span><span class="sxs-lookup"><span data-stu-id="77c9d-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="77c9d-116">Устройството е Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="77c9d-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="77c9d-117">Само Windows 10 Pro, образование и корпоративните skus могат да се присъединят към Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77c9d-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="77c9d-118">Допълнителни ресурси за разрешаване на проблема:</span><span class="sxs-lookup"><span data-stu-id="77c9d-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="77c9d-119">Използвайте [Intune Отстраняване на неизправности портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на често срещани записване грешки.</span><span class="sxs-lookup"><span data-stu-id="77c9d-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="77c9d-120">Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="77c9d-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="77c9d-121">Прегледайте тези документи за списък с често срещани грешки, които пречат на записване и решения за всеки от тях: [Ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и отстраняване на неизправности [.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="77c9d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="77c9d-122">[Научете как да записвате устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="77c9d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
