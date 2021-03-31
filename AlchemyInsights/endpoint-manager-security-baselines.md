---
title: Диспечер на EndPoint – Базови линии за защита
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440864"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="69c7d-102">Диспечер на EndPoint – Базови линии за защита</span><span class="sxs-lookup"><span data-stu-id="69c7d-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="69c7d-103">Базовите линии за защита са предварително конфигурирани групи от настройки на Windows, които ви помагат да приложите настройките за защита, препоръчани от съответните екипи за защита.</span><span class="sxs-lookup"><span data-stu-id="69c7d-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="69c7d-104">Тези базови линии могат да бъдат персонализирани, за да предоставят само желаните настройки и стойности.</span><span class="sxs-lookup"><span data-stu-id="69c7d-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="69c7d-105">За повече информация относно базовите линии на защитата вж. [Използване на базови линии за защита за конфигуриране на устройства с Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="69c7d-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="69c7d-106">В момента има базови линии за тези продукти:</span><span class="sxs-lookup"><span data-stu-id="69c7d-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="69c7d-107">Настройки за защита на Windows MDM</span><span class="sxs-lookup"><span data-stu-id="69c7d-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="69c7d-108">Защита за Microsoft Defender за крайна точка</span><span class="sxs-lookup"><span data-stu-id="69c7d-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="69c7d-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="69c7d-109">Microsoft Edge</span></span>

<span data-ttu-id="69c7d-110">Всяка от базовите линии се актуализира периодично и се издава в постъпкови версии.</span><span class="sxs-lookup"><span data-stu-id="69c7d-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="69c7d-111">Всяка версия добавя и/или премахва настройки от предишната версия, за да гарантира, че базовата линия отговаря на текущите указания.</span><span class="sxs-lookup"><span data-stu-id="69c7d-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="69c7d-112">Конзолата за базова линия на защита в защитата на Endpoint позволява да се сравняват различни версии, като прави промените от версия към версия видими.</span><span class="sxs-lookup"><span data-stu-id="69c7d-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="69c7d-113">За указания как най-ефективно да промените коя версия на базова линия е разположена, вижте [Управление на профилите на базови линии на защита в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="69c7d-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="69c7d-114">След разполагането на базова линия на защита можете да следите състоянието на разполагане и да преглеждате настройките „устройство по устройство“.</span><span class="sxs-lookup"><span data-stu-id="69c7d-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="69c7d-115">**Забележка:** Възможно е да са необходими до 24 часа, за да се покажат данните за отчитане на базови линии – от първоначалното разполагане до устройство и до 6 часа за по-нататъшни актуализации.</span><span class="sxs-lookup"><span data-stu-id="69c7d-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="69c7d-116">Най-често срещаната причина за неприложимата настройка на базова линия е, защото същата настройка се използва в друг профил.</span><span class="sxs-lookup"><span data-stu-id="69c7d-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="69c7d-117">Този сценарий може да бъде изследван за конкретно устройство, като се избере това устройство от възела „Състояние на устройството“ на профила „Базова линия на защита“.</span><span class="sxs-lookup"><span data-stu-id="69c7d-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="69c7d-118">За подробности вж. [Разрешаване на конфликти за базови линии на защита](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="69c7d-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>