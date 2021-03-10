---
title: Използване на базовите линии за защита на Microsoft за конфигуриране на устройства с Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50692905"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="d2899-102">Използване на базовите линии за защита на Microsoft за конфигуриране на устройства с Windows 10</span><span class="sxs-lookup"><span data-stu-id="d2899-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="d2899-103">Настройването на базовите линии за защита помага за защитата на потребителите и устройствата.</span><span class="sxs-lookup"><span data-stu-id="d2899-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="d2899-104">Базовите линии за защита са настройките на Windows предварително конфигурирани групи, използвани за прилагане на известна група настройки и стойности по подразбиране, Препоръчани от съответните екипи за защита.</span><span class="sxs-lookup"><span data-stu-id="d2899-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="d2899-105">Чрез създаване на профил на базова линия за защита, можете да създадете шаблон, който се състои от няколко профила за конфигуриране на устройството.</span><span class="sxs-lookup"><span data-stu-id="d2899-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="d2899-106">Когато разположите базови линии за защита на групи от потребители или устройства, настройките се прилагат към устройства, които работят с Windows 10 или по-нови версии.</span><span class="sxs-lookup"><span data-stu-id="d2899-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="d2899-107">Например базовата линия за управление на Microsoft Mobile devices (MDM) автоматично (1) разрешава защитено стартиране за сменяеми устройства (2) изисква паролата за отключване на устройство и (3) забранява основното удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="d2899-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="d2899-108">Когато стойността по подразбиране не работи за вашата среда, можете да персонализирате базовата линия, за да приложите желаните от вас настройки.</span><span class="sxs-lookup"><span data-stu-id="d2899-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="d2899-109">Базовите линии за защита допринасят и за създаването на защитен работен поток от край до край в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d2899-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="d2899-110">По-долу са дадени някои предимства на тази функция:</span><span class="sxs-lookup"><span data-stu-id="d2899-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="d2899-111">Базовата линия за защита включва най-добрите практики и препоръки за настройките, които оказват влияние върху сигурността.</span><span class="sxs-lookup"><span data-stu-id="d2899-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="d2899-112">Тъй като събеседниците ви са партньори с екипа за защита на Windows, който създава базови линии за групови правила, тези препоръки се основават на солидна ориентация и обширна среда за работа.</span><span class="sxs-lookup"><span data-stu-id="d2899-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="d2899-113">Ако не сте нови и не сте сигурни къде да започнете, тогава основните линии за защита ще ви помогнат бързо да създадете и разположите защитен профил.</span><span class="sxs-lookup"><span data-stu-id="d2899-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="d2899-114">Ако в момента използвате групови правила, тогава преминаването към настройки за целите на управлението е много по-лесно с базовите линии за защита, тъй като тези базови линии за защита са вградени в една и съща функция за управление.</span><span class="sxs-lookup"><span data-stu-id="d2899-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="d2899-115">За повече информация вижте [базови линии](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) и управление на [мобилни устройства](https://docs.microsoft.com/windows/client-management/mdm/)в Windows.</span><span class="sxs-lookup"><span data-stu-id="d2899-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>