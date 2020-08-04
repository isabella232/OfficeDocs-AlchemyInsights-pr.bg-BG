---
title: Свързани с VPN въпроси
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554741"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="dca93-102">Свързани с VPN въпроси</span><span class="sxs-lookup"><span data-stu-id="dca93-102">VPN related issues</span></span>

<span data-ttu-id="dca93-103">Успешното внедряване на VPN свързаност за MDM клиенти зависи от разположения профил, който отразява правилно изискванията на VPN инфраструктурата.</span><span class="sxs-lookup"><span data-stu-id="dca93-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="dca93-104">За подходящите настройки за клиентските платформи, които проучвате, вижте:</span><span class="sxs-lookup"><span data-stu-id="dca93-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="dca93-105">Настройките на Windows 10 и Holographic устройства за добавяне на VPN връзки с помощта на Intune</span><span class="sxs-lookup"><span data-stu-id="dca93-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="dca93-106">Добавяне на vpn настройки на iOS и iPadOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dca93-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="dca93-107">Настройки на устройството с Android, за да конфигурирате VPN в Intune</span><span class="sxs-lookup"><span data-stu-id="dca93-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="dca93-108">Добавяне на VPN настройки на macOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dca93-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="dca93-109">Ако вашият ПРОФИЛ VPN използва удостоверяване, базирано на сертификат, уверете се, че профилите на главния сертификат и сертификат за удостоверяване на клиент, свързани с профила на VPN са разположени успешно.</span><span class="sxs-lookup"><span data-stu-id="dca93-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="dca93-110">**Често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="dca93-110">**Common Issues**</span></span>

<span data-ttu-id="dca93-111">**Внедрих профил в VPN на устройство. Intune показва, че е бил успешен, но устройството не се свързва с VPN.**</span><span class="sxs-lookup"><span data-stu-id="dca93-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="dca93-112">Успешно състояние означава, че Intune успешно внедри профила като конфигуриран.</span><span class="sxs-lookup"><span data-stu-id="dca93-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="dca93-113">Тези конфигурации обаче може да не отговарят на изискванията за мрежата и/или удостоверяването.</span><span class="sxs-lookup"><span data-stu-id="dca93-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="dca93-114">Преглед на регистрите в инфраструктура и удостоверяване услугата (на VPN сървъра и NPS/Radius сървър) за повече информация за опит за връзка.</span><span class="sxs-lookup"><span data-stu-id="dca93-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="dca93-115">Може да се наложи да работите с екипа на мрежовата инфраструктура или доставчика на VPN на трета страна, за да съберете и прегледате трупите.</span><span class="sxs-lookup"><span data-stu-id="dca93-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="dca93-116">**Когато конфигурирам персонализирана VPN за iOS, vpn функцията за всеки app не е налична.**</span><span class="sxs-lookup"><span data-stu-id="dca93-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="dca93-117">В момента е достъпен за конкретен списък от доставчици и партньори, които трябва да отговарят на предварителните изисквания за сертификата, преди да конфигурират VPN услуга за приложение.</span><span class="sxs-lookup"><span data-stu-id="dca93-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="dca93-118">За повече информация вижте [Настройване на виртуална частна мрежа за iOS/iPadOS в Intune.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="dca93-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="dca93-119">За повече информация за всички видове VPN връзки в Intune вижте [Създаване на VPN профили за свързване с VPN сървъри в Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="dca93-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="dca93-120">**iOS По заявка VPN не се задейства, когато конфигуриран домейн е достъпна**</span><span class="sxs-lookup"><span data-stu-id="dca93-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="dca93-121">За да тествате автоматичните настройки на VPN, задайте следните стойности:</span><span class="sxs-lookup"><span data-stu-id="dca93-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="dca93-122">Искам да направя следното: Оценка на **всеки опит за свързване**</span><span class="sxs-lookup"><span data-stu-id="dca93-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="dca93-123">Изберете дали да се свържете: **Свържете се, ако е необходимо**</span><span class="sxs-lookup"><span data-stu-id="dca93-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="dca93-124">Когато потребителите имат достъп до тези домейни: **целеви** *домейн*</span><span class="sxs-lookup"><span data-stu-id="dca93-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="dca93-125">Ако горната конфигурация не е успешна, добавете следния елемент:</span><span class="sxs-lookup"><span data-stu-id="dca93-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="dca93-126">Когато този URL адрес е недостъпен, сила свържете VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="dca93-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>