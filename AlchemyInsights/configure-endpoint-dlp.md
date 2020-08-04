---
title: Конфигуриране на крайна точка DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/03/2020
ms.locfileid: "46554815"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="5e60e-102">Конфигуриране на крайна точка DLP</span><span class="sxs-lookup"><span data-stu-id="5e60e-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="5e60e-103">Microsoft Endpoint DLP ви позволява да разширите DLP защита и възможност за наблюдение на поверителна информация на устройства с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5e60e-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="5e60e-104">След като устройствата се качват в управлението на устройства, можете да създадете DLP правила за прилагане на защитни действия за елементи.</span><span class="sxs-lookup"><span data-stu-id="5e60e-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="5e60e-105">Мениджърът на дейности може да се използва за наблюдение на дейността за чувствителни елементи.</span><span class="sxs-lookup"><span data-stu-id="5e60e-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="5e60e-106">За повече информация вижте [Устройства за включване в управлението на устройства](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="5e60e-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="5e60e-107">За да започнете с DLP за крайна точка:</span><span class="sxs-lookup"><span data-stu-id="5e60e-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="5e60e-108">Уверете се, че имате подходящи лицензи за sku/абонаменти.</span><span class="sxs-lookup"><span data-stu-id="5e60e-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="5e60e-109">За повече информация вижте [лицензиране на SKU/абонаменти](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="5e60e-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="5e60e-110">Проверете разрешенията, необходими за разрешаване на управлението на устройства, достъп до страницата за включване или включване/изключване на наблюдението на устройства.</span><span class="sxs-lookup"><span data-stu-id="5e60e-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="5e60e-111">За повече информация вижте [Разрешения](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="5e60e-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="5e60e-112">Бордови устройства в управление на устройствата, като следвате процедурата за бордови устройства.</span><span class="sxs-lookup"><span data-stu-id="5e60e-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="5e60e-113">Ако липсва опцията Device Onboarding (преглед) под M365 **съответствие настройки**, потвърдете, че имате подходящия лиценз и разрешения, посочени по-горе.</span><span class="sxs-lookup"><span data-stu-id="5e60e-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="5e60e-114">За повече информация вижте [Устройства за включване](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="5e60e-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="5e60e-115">Създаване на правила за DLP за защита на вашите поверителни елементи.</span><span class="sxs-lookup"><span data-stu-id="5e60e-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="5e60e-116">За информация вижте [Сценарии за DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)за крайна точка .</span><span class="sxs-lookup"><span data-stu-id="5e60e-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="5e60e-117">За повече информация относно DLP на крайна точка на Microsoft вижте [Научете за Microsoft 365 крайни данни загуба предотвратяване (визуализация)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="5e60e-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>