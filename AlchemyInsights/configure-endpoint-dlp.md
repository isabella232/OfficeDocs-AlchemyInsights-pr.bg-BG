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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657918"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="eb8e1-102">Конфигуриране на DLP на крайна точка</span><span class="sxs-lookup"><span data-stu-id="eb8e1-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="eb8e1-103">DLP на крайна точка на Microsoft ви позволява да разширите възможностите за DLP защита и наблюдение за чувствителна информация на устройства с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="eb8e1-104">След като устройствата се регистрират в управлението на устройства, можете да създадете DLP правила, за да приложите защитни действия върху елементи.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="eb8e1-105">„Преглед на дейността“ може да се използва за наблюдение на дейността при чувствителни елементи.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="eb8e1-106">За повече информация вж. [Регистриране на устройства в управлението на устройства](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="eb8e1-107">За да започнете с DLP за крайна точка:</span><span class="sxs-lookup"><span data-stu-id="eb8e1-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="eb8e1-108">Уверете се, че имате съответния лиценз за ИЕ/абонамент.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="eb8e1-109">За повече информация вж. [лицензи за ИЕ/абонаменти](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="eb8e1-110">Проверете разрешенията, необходими за разрешаване на управлението на устройства, достъпа до страницата за регистриране или включване/изключване на наблюдението на устройства.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="eb8e1-111">За повече информация вж. [Разрешения](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="eb8e1-112">Регистрирайте устройствата в управлението на устройства, като се следвате процедурата за регистриране на устройства.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="eb8e1-113">За повече информация вж. [Регистриране на устройства](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="eb8e1-114">Създайте DLP правила, за да защитите своите чувствителни елементи.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="eb8e1-115">За информация вж. [Сценарии за DLP правила за крайна точка](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="eb8e1-116">За повече информация относно DLP за крайна точка на Microsoft вж. [Научете за защитата от загуба на данни на крайна точка на Microsoft 365 (предварителен преглед)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="eb8e1-117">**Важни стъпки за събиране на данни, ако е необходима поддръжка:**</span><span class="sxs-lookup"><span data-stu-id="eb8e1-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="eb8e1-118">Изтегляне [на визуализация на анализатора на клиенти на MDATP](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="eb8e1-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="eb8e1-119">Изпълнете инструмента като администратор от командния прозорец:</span><span class="sxs-lookup"><span data-stu-id="eb8e1-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="eb8e1-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="eb8e1-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="eb8e1-121">Когато получите подкана с **Въведете броя минути, за да съберете проследявания:** въведете броя минути, необходими за изпълнение на сценария.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="eb8e1-122">Изпълнете сценария.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-122">Run the scenario.</span></span>

<span data-ttu-id="eb8e1-123">Съберете изходния файл zip, за да дадете на агента по поддръжката.</span><span class="sxs-lookup"><span data-stu-id="eb8e1-123">Collect the Zip file output to give to the Support agent.</span></span>
