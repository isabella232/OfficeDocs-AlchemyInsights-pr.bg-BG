---
title: EndPoint Manager – базови стойности на защитата
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420720"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="45d28-102">EndPoint Manager – базови стойности на защитата</span><span class="sxs-lookup"><span data-stu-id="45d28-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="45d28-103">Базовите стойности на защитата са предварително конфигурирани групи от настройки на Windows, които ви помагат да приложите настройките за защита, препоръчани от съответните екипи за защита.</span><span class="sxs-lookup"><span data-stu-id="45d28-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="45d28-104">Тези базови стойности могат да бъдат персонализирани, за да предоставят само желаните настройки и стойности.</span><span class="sxs-lookup"><span data-stu-id="45d28-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="45d28-105">За повече информация относно базовите стойности на защитата вижте Използване на базови стойности на защитата за конфигуриране на [устройства с Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="45d28-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="45d28-106">В момента има базови стойности за тези продукти:</span><span class="sxs-lookup"><span data-stu-id="45d28-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="45d28-107">Настройки за MDM защита на Windows</span><span class="sxs-lookup"><span data-stu-id="45d28-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="45d28-108">Microsoft Defender за защитата на EndPoint</span><span class="sxs-lookup"><span data-stu-id="45d28-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="45d28-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="45d28-109">Microsoft Edge</span></span>

<span data-ttu-id="45d28-110">Всяка от базовите стойности се актуализира периодично и се издава в постъпкови версии.</span><span class="sxs-lookup"><span data-stu-id="45d28-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="45d28-111">Всяка версия добавя и премахва или премахва настройки от предишната версия, за да се гарантира, че базовата линия отговаря на текущите указания.</span><span class="sxs-lookup"><span data-stu-id="45d28-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="45d28-112">Конзолата за базови линии на защитата в Endpoint Security позволява да се сравняват различни версии, като промените от версията към версията се виждат.</span><span class="sxs-lookup"><span data-stu-id="45d28-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="45d28-113">За указания как да промените най-ефективно коя версия на базовата линия е разположена, вижте Управление на базовите профили за [защита в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="45d28-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="45d28-114">След разполагането на базова стойност на защитата можете да следите състоянието на разполагане и да преглеждате настройките на базата на устройство по устройство.</span><span class="sxs-lookup"><span data-stu-id="45d28-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="45d28-115">**Забележка:** Данните за отчитане за базовите стойности може да отнемат до 24 часа, за да се покажат от първоначалното разполагане до устройство и до 6 часа за по-нататъшни актуализации.</span><span class="sxs-lookup"><span data-stu-id="45d28-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="45d28-116">Най-често срещаната причина за базова настройка, която не се прилага, е, че същата настройка се използва в друг профил.</span><span class="sxs-lookup"><span data-stu-id="45d28-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="45d28-117">Този сценарий може да бъде изследван за конкретно устройство, като изберете това устройство от възела Състояние на устройството на профила на базовата линия на защитата.</span><span class="sxs-lookup"><span data-stu-id="45d28-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="45d28-118">За подробности вижте Разрешаване [на конфликти за базови стойности на защитата.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="45d28-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>