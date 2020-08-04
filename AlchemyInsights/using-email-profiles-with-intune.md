---
title: Използване на имейл профили с Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554743"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="76d88-102">Използване на имейл профили с Intune</span><span class="sxs-lookup"><span data-stu-id="76d88-102">Using email profiles with Intune</span></span>

<span data-ttu-id="76d88-103">Intune може да се използва за създаване и внедряване на имейл профили за основен (вграден) имейл клиент на няколко платформи на устройства.</span><span class="sxs-lookup"><span data-stu-id="76d88-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="76d88-104">За информация относно някои от ограниченията, свързани с имейл профили, включително как се обработват съществуващите профили и как се премахват имейл профилите, вижте [Добавяне на настройки за имейл към устройства, използващи Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="76d88-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="76d88-105">За повече информация относно създаването на имейл профили за всяка платформа на устройството вижте:</span><span class="sxs-lookup"><span data-stu-id="76d88-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="76d88-106">Настройки на устройството с Android за конфигуриране на имейл, удостоверяване и синхронизиране в Intune</span><span class="sxs-lookup"><span data-stu-id="76d88-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="76d88-107">Добавяне на настройки за електронна поща за iOS и iPadOS устройства в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="76d88-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="76d88-108">Настройки на имейл профил в Microsoft Intune за устройства с Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="76d88-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="76d88-109">Настройки на имейл профила за устройства с Windows 10 в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="76d88-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="76d88-110">**Често срещан проблем при синхронизиране**</span><span class="sxs-lookup"><span data-stu-id="76d88-110">**Common syncing issue**</span></span>

<span data-ttu-id="76d88-111">**KNOX в имейл профила на Android не позволява на потребителски контакти, календар и задачи, синхронизиране на потребителски устройства.**</span><span class="sxs-lookup"><span data-stu-id="76d88-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="76d88-112">В KNOX на Android KNOX имейл профил предлага на администратора възможност да реши кои типове съдържание са синхронизирани на устройството чрез настройка всеки да е активиран.</span><span class="sxs-lookup"><span data-stu-id="76d88-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="76d88-113">Ако настройката за някой от типовете съдържание е зададена на **Не е конфигуриран** (по подразбиране), този тип съдържание не е синхронизиран автоматично.</span><span class="sxs-lookup"><span data-stu-id="76d88-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="76d88-114">Потребителят може да разреши типа на съдържанието, който иска ръчно директно на устройството, но тази конфигурация се замества от настройката на правилата на Intune и синхронизирането спира за този тип съдържание.</span><span class="sxs-lookup"><span data-stu-id="76d88-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

