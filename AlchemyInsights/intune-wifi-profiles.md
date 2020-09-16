---
title: Настройване на Wi-Fi профили
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696250"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="f2f9a-102">Настройване на Wi-Fi профили</span><span class="sxs-lookup"><span data-stu-id="f2f9a-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="f2f9a-103">Успешното реализиране на Wi-Fi връзка за MDM клиенти зависи от правилно разположен профил, който отговаря на изискванията на корпоративната Wi-Fi инфраструктура.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="f2f9a-104">За да прегледате подходящите настройки за клиентските платформи, които разследвате, вижте:</span><span class="sxs-lookup"><span data-stu-id="f2f9a-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="f2f9a-105">Добавяне на Wi-Fi настройки за устройства, работещи с Android в Microsoft за настройка</span><span class="sxs-lookup"><span data-stu-id="f2f9a-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="f2f9a-106">Добавяне на Wi-Fi настройки за устройства, посветени на Android Enterprise, както и за цялостно управление в Microsoft</span><span class="sxs-lookup"><span data-stu-id="f2f9a-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="f2f9a-107">Добавяне на Wi-Fi настройки за устройства с iOS и iPadOS в Microsoft за настройка</span><span class="sxs-lookup"><span data-stu-id="f2f9a-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="f2f9a-108">Добавяне на Wi-Fi настройки за устройства с Windows 10 и по-нови версии</span><span class="sxs-lookup"><span data-stu-id="f2f9a-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="f2f9a-109">Импортиране на Wi-Fi настройки за устройства с Windows в съзвучие</span><span class="sxs-lookup"><span data-stu-id="f2f9a-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="f2f9a-110">**Често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="f2f9a-110">**Common Issues**</span></span>

<span data-ttu-id="f2f9a-111">**Разполагам с Wi-Fi профил, който зависи от вградения сертификат, зададен в Wi-Fi профила. Профилите на конфигурацията обаче показват състоянието на грешката.**</span><span class="sxs-lookup"><span data-stu-id="f2f9a-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="f2f9a-112">Проверете дали вашето устройство е получило сертификата.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="f2f9a-113">В настройка отидете на **всички устройства** и изберете конфигурацията на устройството > на **устройството**.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="f2f9a-114">Проверете дали всички очаквания профили са посочени и в успешно състояние.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="f2f9a-115">За профил на Android, ако имате междинни сертификати във вашата верига на сертификати, се уверете, че те са разположени на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="f2f9a-116">За да проверите състоянието на сертификата, отидете на профили за **Конфигуриране на устройства**с Android, за да имате  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **надежден сертификат**за свойства.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="f2f9a-117">Ако продължавате да виждате грешки, прегледайте разделите процедури и отстраняване на неизправности.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="f2f9a-118">За повече информация вижте [общ преглед за отстраняване на неизправности в профилите на SCEP с Microsoft](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f2f9a-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="f2f9a-119">**Разполагам с Wi-Fi профил към устройство. Тази информация показва, че е била успешна, но устройството не се свързва с Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="f2f9a-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="f2f9a-120">Успешната задача означава, че в този случай е успешно разгърнат профилът, както е конфигуриран.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="f2f9a-121">Тези конфигурации обаче може да не отговарят на вашите изисквания за мрежа и/или удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="f2f9a-122">За повече информация относно опитните връзки прегледайте регистрите в услугата инфраструктура и удостоверяване (на администратора на Wi-Fi точка за достъп и на сървъра за НП).</span><span class="sxs-lookup"><span data-stu-id="f2f9a-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="f2f9a-123">Може да се наложи да работите с вашия екип за мрежова инфраструктура или с доставчика на Wi-Fi на друг доставчик, за да събирате и преглеждате регистрационни файлове.</span><span class="sxs-lookup"><span data-stu-id="f2f9a-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>