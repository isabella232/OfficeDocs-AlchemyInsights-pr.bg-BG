---
title: Използване на базови линии за защита на Microsoft за конфигуриране на устройства с Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573282"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="72850-102">Използване на базови линии за защита на Microsoft за конфигуриране на устройства с Windows 10</span><span class="sxs-lookup"><span data-stu-id="72850-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="72850-103">Настройването на базовите линии за защита помага за защитата на потребителите и устройствата.</span><span class="sxs-lookup"><span data-stu-id="72850-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="72850-104">Базовите линии за защита са настройките на Windows предварително конфигурирани групи, използвани за прилагане на известна група настройки и стойности по подразбиране, Препоръчани от съответните екипи за защита.</span><span class="sxs-lookup"><span data-stu-id="72850-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="72850-105">Чрез създаване на профил на базова линия за защита, можете да създадете шаблон, който се състои от няколко профила за конфигуриране на устройството.</span><span class="sxs-lookup"><span data-stu-id="72850-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="72850-106">Когато разположите базови линии за защита на групи от потребители или устройства, настройките се прилагат към устройства, които се изпълняват на Windows 10 или по-нови версии.</span><span class="sxs-lookup"><span data-stu-id="72850-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="72850-107">Например MDM базовата линия за защита автоматично (1) разрешава BitLocker за сменяеми устройства (2) изисква паролата за отключване на устройство и (3) забранява основното удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="72850-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="72850-108">Когато стойността по подразбиране не работи за вашата среда, Персонализирайте базовата линия, за да приложите желаните от вас настройки.</span><span class="sxs-lookup"><span data-stu-id="72850-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="72850-109">Базовите линии за защита допринасят и за създаването на защитен работен поток от край до край в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72850-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="72850-110">По-долу са дадени някои предимства на това:</span><span class="sxs-lookup"><span data-stu-id="72850-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="72850-111">Базовата линия за защита включва най-добрите практики и препоръки за настройките, които оказват влияние върху сигурността.</span><span class="sxs-lookup"><span data-stu-id="72850-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="72850-112">Тъй като събеседниците ви са партньори с екипа за защита на Windows, който създава базови линии за групови правила, тези препоръки се основават на солидна ориентация и обширна среда за работа.</span><span class="sxs-lookup"><span data-stu-id="72850-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="72850-113">Ако не сте нови и не сте сигурни къде да започнете, тогава основните линии за защита ще ви помогнат бързо да създадете и разположите защитен профил.</span><span class="sxs-lookup"><span data-stu-id="72850-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="72850-114">Ако в момента използвате групови правила, тогава преминаването към настройки за целите на управлението е много по-лесно с базовите линии за защита, тъй като те са вградени в "Настройки" и включват възможностите за авангарден мениджмънт за управлението.</span><span class="sxs-lookup"><span data-stu-id="72850-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="72850-115">За да научите повече, вижте [базови линии](https://go.microsoft.com/fwlink/?linkid=2141503) и [управление на мобилни устройства](https://go.microsoft.com/fwlink/?linkid=2141701)в Windows.</span><span class="sxs-lookup"><span data-stu-id="72850-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>