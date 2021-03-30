---
title: Конфигуриране на DLP на крайна точка
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402402"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="7ed4f-102">Конфигуриране на DLP на крайна точка</span><span class="sxs-lookup"><span data-stu-id="7ed4f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="7ed4f-103">DLP на крайна точка на Microsoft ви позволява да разширите възможностите за DLP защита и наблюдение за чувствителна информация на устройства с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="7ed4f-104">След като устройствата се регистрират в управлението на устройства, можете да създадете DLP правила, за да приложите защитни действия върху елементи.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="7ed4f-105">„Преглед на дейността“ може да се използва за наблюдение на дейността при чувствителни елементи.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="7ed4f-106">За повече информация вж. [Регистриране на устройства в управлението на устройства](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="7ed4f-107">За да започнете с DLP за крайна точка:</span><span class="sxs-lookup"><span data-stu-id="7ed4f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="7ed4f-108">Уверете се, че имате съответния лиценз за ИЕ/абонамент.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="7ed4f-109">За повече информация вж. [лицензи за ИЕ/абонаменти](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="7ed4f-110">Проверете разрешенията, необходими за разрешаване на управлението на устройства, достъпа до страницата за регистриране или включване/изключване на наблюдението на устройства.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="7ed4f-111">За повече информация вж. [Разрешения](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="7ed4f-112">Регистрирайте устройствата в управлението на устройства, като се следвате процедурата за регистриране на устройства.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="7ed4f-113">Ако ви липсва опцията за внедряване на устройството (предварителен преглед) под настройките за съответствие на M365  **Настройки**, уверете се, че имате съответните лицензи и разрешения, посочени по-горе.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="7ed4f-114">За повече информация вж. [Регистриране на устройства](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="7ed4f-115">Създайте DLP правила, за да защитите своите чувствителни елементи.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="7ed4f-116">За информация вж. [Сценарии за DLP правила за крайна точка](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="7ed4f-117">За повече информация относно DLP за крайна точка на Microsoft вж. [Научете за защитата от загуба на данни на крайна точка на Microsoft 365 (предварителен преглед)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="7ed4f-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="7ed4f-118">**Важни стъпки за събиране на данни, ако е необходима поддръжка:**</span><span class="sxs-lookup"><span data-stu-id="7ed4f-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="7ed4f-119">Изтегляне на предварителния преглед на MDATP анализатор на клиента от [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="7ed4f-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="7ed4f-120">Изпълнете инструмента като администратор от командния прозорец:</span><span class="sxs-lookup"><span data-stu-id="7ed4f-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="7ed4f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="7ed4f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="7ed4f-122">Когато получите подкана за "Въвеждане на броя минути, за събиране на проследявания: ", въведете броя минути, които са необходими за изпълнение на сценария</span><span class="sxs-lookup"><span data-stu-id="7ed4f-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="7ed4f-123">Изпълнение на сценария</span><span class="sxs-lookup"><span data-stu-id="7ed4f-123">Run the scenario</span></span>

<span data-ttu-id="7ed4f-124">Съберете изходния zip файл, който да се предаде на агента по поддръжката.</span><span class="sxs-lookup"><span data-stu-id="7ed4f-124">Collect the Zip file output to be given to the Support agent.</span></span>
