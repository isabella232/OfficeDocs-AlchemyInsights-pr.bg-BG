---
title: Използвайте Microsoft Intune базови стойности за защита, за да конфигурирате Windows 10 устройства
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793564"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="7d0ac-102">Използвайте Microsoft Intune базови стойности за защита, за да конфигурирате Windows 10 устройства</span><span class="sxs-lookup"><span data-stu-id="7d0ac-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="7d0ac-103">Базовите стойности на защитата intune помагат за защитата на потребителите и устройствата.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="7d0ac-104">Базовите стойности на защитата Windows предварително конфигурирани групи, използвани за прилагане на известна група от настройки и стойности по подразбиране, препоръчани от съответните екипи за защита.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="7d0ac-105">Чрез създаването на профил на базова линия на защитата в Intune създавате шаблон, който се състои от множество профили за конфигуриране на устройства.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="7d0ac-106">Когато разположите базови стойности на защитата за групи потребители или устройства, настройките се прилагат към устройства, които се изпълняват Windows 10 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="7d0ac-107">Например базовата стойност на защитата на microsoft mobile device management (MDM) автоматично разрешава BitLocker за сменяеми устройства, изисква паролата за отключване на устройство и забранява базовото удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="7d0ac-108">Когато стойността по подразбиране не работи за вашата среда, можете да персонализирате базовата линия, за да приложите нужните настройки.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="7d0ac-109">Базовите стойности на защитата също така помагат за създаването на защитен работен поток от край до край в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="7d0ac-110">Базовата стойност на защитата включва най-добрите практики и препоръки за настройки, които засягат защитата.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="7d0ac-111">Intune partners with the Windows за защита, който създава базови стойности за групови правила, така че тези препоръки се базират на солидни указания и богата среда за работа.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="7d0ac-112">Ако сте нови в Intune и не сте сигурни откъде да започнете, базовите стойности на защитата ви помагат бързо да създадете и разположите защитен профил.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="7d0ac-113">Ако в момента използвате групови правила, мигрирането към Intune за целите на управлението е много по-лесно с базовите стойности на защитата, тъй като те са вградени в Intune и включват най-новите възможности за управление.</span><span class="sxs-lookup"><span data-stu-id="7d0ac-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="7d0ac-114">За да научите повече, [вижте Windows базовите стойности на защитата и](/windows/security/threat-protection/windows-security-baselines) [управлението на мобилни устройства.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="7d0ac-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

