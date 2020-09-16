---
title: Проблеми, свързани с VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726080"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="41d52-102">Проблеми, свързани с VPN</span><span class="sxs-lookup"><span data-stu-id="41d52-102">VPN related issues</span></span>

<span data-ttu-id="41d52-103">Успешното реализиране на VPN свързване за MDM клиенти зависи от разгърнат профил, който отразява правилно изискванията за VPN инфраструктурата.</span><span class="sxs-lookup"><span data-stu-id="41d52-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="41d52-104">За подходящите настройки за клиентските платформи, които разследвате, вижте:</span><span class="sxs-lookup"><span data-stu-id="41d52-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="41d52-105">Настройки на Windows 10 и холографски устройства с Windows, за да добавяте VPN връзки чрез настройка</span><span class="sxs-lookup"><span data-stu-id="41d52-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="41d52-106">Добавяне на настройки за VPN на устройства с iOS и iPadOS в Microsoft за настройка</span><span class="sxs-lookup"><span data-stu-id="41d52-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="41d52-107">Настройки на устройства с Android, за да конфигурирате VPN в съзвучие</span><span class="sxs-lookup"><span data-stu-id="41d52-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="41d52-108">Добавяне на настройки за VPN на устройства macOS в Microsoft</span><span class="sxs-lookup"><span data-stu-id="41d52-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="41d52-109">Ако вашият VPN профил използва удостоверяване, базирано на сертификат, уверете се, че профилите на сертификата за главен сертификат и сертификат за удостоверяване на клиента, свързани с профила за VPN, са разположени успешно.</span><span class="sxs-lookup"><span data-stu-id="41d52-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="41d52-110">**Често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="41d52-110">**Common Issues**</span></span>

<span data-ttu-id="41d52-111">**Разположих профил за VPN към устройство. Тази информация показва, че е била успешна, но устройството не се свързва към VPN.**</span><span class="sxs-lookup"><span data-stu-id="41d52-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="41d52-112">Успешната задача означава, че в този случай е успешно разгърнат профилът, както е конфигуриран.</span><span class="sxs-lookup"><span data-stu-id="41d52-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="41d52-113">Тези конфигурации обаче може да не отговарят на вашите изисквания за мрежа и/или удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="41d52-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="41d52-114">Преглеждане на регистрационни файлове в услугата инфраструктура и удостоверяване (на сървъра за VPN и НП/радиус Server) за повече подробности относно опита за свързване.</span><span class="sxs-lookup"><span data-stu-id="41d52-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="41d52-115">Може да се наложи да работите с вашия екип за мрежова инфраструктура или с доставчика на VPN от друга страна, за да събирате и преглеждате регистрационни файлове.</span><span class="sxs-lookup"><span data-stu-id="41d52-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="41d52-116">**Когато конфигурирам потребителски VPN за iOS, функцията за VPN за приложения не се предлага.**</span><span class="sxs-lookup"><span data-stu-id="41d52-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="41d52-117">За приложенията VPN за устройства с iOS, в момента се предлага за конкретен списък с доставчици и партньори, които трябва също да отговарят на предварителните изисквания за сертификатите, преди да конфигурират VPN за приложения.</span><span class="sxs-lookup"><span data-stu-id="41d52-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="41d52-118">За повече информация вижте [Настройване на виртуални частни мрежи (VPN) за устройства с IOS/iPadOS в съзвучие](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="41d52-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="41d52-119">За повече информация за всички типове VPN връзки в настройки вижте [Създаване на VPN профили, за да се свържете към сървърите на VPN в съзвучие](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="41d52-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="41d52-120">**VPN при заявка с iOS не се задейства при достъп до конфигуриран домейн**</span><span class="sxs-lookup"><span data-stu-id="41d52-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="41d52-121">За да изпробвате настройките за автоматични VPN, Задайте следните стойности:</span><span class="sxs-lookup"><span data-stu-id="41d52-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="41d52-122">Искам да направя следното: **оценявай всеки опит за свързване**</span><span class="sxs-lookup"><span data-stu-id="41d52-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="41d52-123">Изберете дали да се свържете: **свързване, ако е необходимо**</span><span class="sxs-lookup"><span data-stu-id="41d52-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="41d52-124">Когато потребителите имат достъп до следните домейни: име на **целевия** *домейн*</span><span class="sxs-lookup"><span data-stu-id="41d52-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="41d52-125">Ако конфигурацията по-горе не е успешна, добавете следния елемент:</span><span class="sxs-lookup"><span data-stu-id="41d52-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="41d52-126">Когато този URL адрес е недостъпен, Force свържете VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="41d52-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>