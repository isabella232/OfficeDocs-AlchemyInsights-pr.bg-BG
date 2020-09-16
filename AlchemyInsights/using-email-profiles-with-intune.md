---
title: Използване на имейл профили с настройки
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653277"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="7c603-102">Използване на имейл профили с настройки</span><span class="sxs-lookup"><span data-stu-id="7c603-102">Using email profiles with Intune</span></span>

<span data-ttu-id="7c603-103">Можете да използвате функцията за създаване и разполагане на имейл профили за собствения (вграден) имейл клиент на множество платформи за устройства.</span><span class="sxs-lookup"><span data-stu-id="7c603-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="7c603-104">За информация относно някои от ограниченията, свързани с имейл профилите, включително как се обработват наличността на съществуващите профили и как се премахват имейл профилите, вижте [Добавяне на имейл настройки към устройства чрез настройка](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="7c603-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="7c603-105">За повече информация как да създадете имейл профили за всяка платформа на устройство, вижте:</span><span class="sxs-lookup"><span data-stu-id="7c603-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="7c603-106">Настройки на устройства с Android, за да конфигурирате имейл, удостоверяване и синхронизиране в съзвучие</span><span class="sxs-lookup"><span data-stu-id="7c603-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="7c603-107">Добавяне на имейл настройки за устройства с iOS и iPadOS в Microsoft за настройка</span><span class="sxs-lookup"><span data-stu-id="7c603-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="7c603-108">Настройки на имейл профил в Microsoft за устройства, на които се изпълнява Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="7c603-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="7c603-109">Настройки на имейл профил за устройства, работещи с Windows 10 в Microsoft за настройка</span><span class="sxs-lookup"><span data-stu-id="7c603-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="7c603-110">**Често срещан проблем при синхронизиране**</span><span class="sxs-lookup"><span data-stu-id="7c603-110">**Common syncing issue**</span></span>

<span data-ttu-id="7c603-111">**Имейл профилът на KNOX в Android позволява на потребителските контакти, календар и задачи да се синхронизират с потребителските устройства.**</span><span class="sxs-lookup"><span data-stu-id="7c603-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="7c603-112">Имейл профилът KNOX на Android KNOX предлага на администратора опцията да реши кои типове съдържание да се синхронизират с устройството, като зададете всеки да е разрешен.</span><span class="sxs-lookup"><span data-stu-id="7c603-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="7c603-113">Ако настройката за който и да е от типовете съдържание е зададена като " **не е конфигурирана** " (по подразбиране), този тип съдържание не се синхронизира автоматично.</span><span class="sxs-lookup"><span data-stu-id="7c603-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="7c603-114">Потребителят може да разреши типа съдържание, който искате директно на устройството, но тази конфигурация е заместена от настройката правила за настройка и синхронизирането спира за този тип съдържание.</span><span class="sxs-lookup"><span data-stu-id="7c603-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

