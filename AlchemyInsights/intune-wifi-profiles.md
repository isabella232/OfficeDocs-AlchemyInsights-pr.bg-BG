---
title: Intune Wi-Fi профили
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554788"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="c0ce1-102">Intune Wi-Fi профили</span><span class="sxs-lookup"><span data-stu-id="c0ce1-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="c0ce1-103">Успешното внедряване на Wi-Fi свързаност за MDM клиенти зависи от правилно разположен профил, който отразява изискванията на корпоративната Wi-Fi инфраструктура.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="c0ce1-104">За да прегледате подходящите настройки за клиентските платформи, които проучвате, вижте:</span><span class="sxs-lookup"><span data-stu-id="c0ce1-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="c0ce1-105">Добавяне на wi-Fi настройки за устройства с Android в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c0ce1-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="c0ce1-106">Добавете Wi-Fi настройки за android Enterprise специализирани и напълно управлявани устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c0ce1-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="c0ce1-107">Добавяне на Wi-Fi настройки за iOS и iPadOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c0ce1-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="c0ce1-108">Добавяне на Wi-Fi настройки за Windows 10 и по-нови устройства в Intune</span><span class="sxs-lookup"><span data-stu-id="c0ce1-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="c0ce1-109">Импортиране на Wi-Fi настройки за устройства с Windows в Intune</span><span class="sxs-lookup"><span data-stu-id="c0ce1-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="c0ce1-110">**Често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="c0ce1-110">**Common Issues**</span></span>

<span data-ttu-id="c0ce1-111">**Разполагам Wi-Fi профил, който зависи от разположени сертификат, посочен в профила за Wi-Fi. Обаче профили за конфигуриране показват състояние на грешка.**</span><span class="sxs-lookup"><span data-stu-id="c0ce1-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="c0ce1-112">Проверете дали устройството ви е получило сертификата.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="c0ce1-113">В Intune отидете на **Всички устройства** и изберете устройството > конфигурация **на устройството**.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="c0ce1-114">Проверете дали всички очаквани профили са изброени и в успешно състояние.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="c0ce1-115">За профил в Android, ако имате междинни сертификати във вашата верига на сертификати, уверете се, че те са разположени на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="c0ce1-116">За да проверите състоянието на сертификата, отидете на **Device Configuration**  >  **Profiles**  >  **Android междинен CA**свойства  >  **Properties**  >  **надежден сертификат**.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="c0ce1-117">Ако продължавате да виждате грешки, прегледайте процедурите и секциите за отстраняване на неизправности.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="c0ce1-118">За повече информация вижте [общ преглед за отстраняване на SCEP сертификат профили с Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c0ce1-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="c0ce1-119">**Разгърнах профил за Wi-Fi към устройство. Intune показва, че е била успешна, но устройството не се свързва с Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="c0ce1-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="c0ce1-120">Успешно състояние означава, че Intune успешно внедри профила като конфигуриран.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="c0ce1-121">Тези конфигурации обаче може да не отговарят на изискванията за мрежата и/или удостоверяването.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="c0ce1-122">За повече информация относно опит за свързване прегледайте регистрационните файлове в инфраструктурата и услугата за удостоверяване (на Wi-Fi точка за достъп контролер и NPS/Radius сървър).</span><span class="sxs-lookup"><span data-stu-id="c0ce1-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="c0ce1-123">Може да се наложи да работите с екипа по мрежова инфраструктура или доставчика на Wi-Fi на трета страна, за да събирате и преглеждате регистрационни файлове.</span><span class="sxs-lookup"><span data-stu-id="c0ce1-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>