---
title: Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353526"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="ff8ce-102">Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ff8ce-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="ff8ce-103">Преглед на ресурси, изброени по-долу да решим вашия проблем сега.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ff8ce-104">Някои често срещани съобщения за грешка и разрешаване стъпки:</span><span class="sxs-lookup"><span data-stu-id="ff8ce-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="ff8ce-105">**Не може да бъде инсталиран софтуер, 0x80cf4017:** Сертификат вашия акаунт е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="ff8ce-106">Повторно изтегляне компютър клиент софтуерен пакет в на Intune административната конзола.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="ff8ce-107">Прегледайте документацията за повече информация.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="ff8ce-108">**Код на грешка 0x801c0003:** Тази грешка може да възникне в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="ff8ce-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="ff8ce-109">Потребителят има повече устройства, записани от лимита за устройството.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ff8ce-110">Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ff8ce-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="ff8ce-111">"Потребителите може да присъедини устройства към лазурните АД" е настроен на "няма".</span><span class="sxs-lookup"><span data-stu-id="ff8ce-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="ff8ce-112">Поставям то към всички или изберете потребители.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-112">Set it to all or select users.</span></span> <span data-ttu-id="ff8ce-113">Прегледайте [документацията](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="ff8ce-114">Устройството вече е записан от друг потребител.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="ff8ce-115">Ако случаят е такъв, премахнете устройството от Azure Intune конзола или ръчно unenroll устройство преди да опитате отново.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="ff8ce-116">Устройството е Windows 10 Начало.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="ff8ce-117">Само Windows 10 Pro, образование и предприятието ие може да обединяват Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="ff8ce-118">Допълнителни ресурси за разрешаване на вашия проблем:</span><span class="sxs-lookup"><span data-stu-id="ff8ce-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ff8ce-119">Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ff8ce-120">Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ff8ce-121">Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [отстраняване на док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ff8ce-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="ff8ce-122">[Научете как да се запишат устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="ff8ce-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
