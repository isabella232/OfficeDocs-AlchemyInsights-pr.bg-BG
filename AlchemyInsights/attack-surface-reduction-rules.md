---
title: Правила за намаляване на повърхността на атака
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676072"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c8bf5-102">Правила за намаляване на повърхността на атака</span><span class="sxs-lookup"><span data-stu-id="c8bf5-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c8bf5-103">Изключването на файлове или папки може сериозно да намали защитата, предоставена от правилата за намаляване на повърхността на атаката.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c8bf5-104">Файловете, които биха били блокирани от правило, могат да се изпълняват и не се записва отчет или събитие.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c8bf5-105">Изключение се отнася за всички правила, които позволяват изключения.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c8bf5-106">Изключенията от ASR използват същия синтаксис като Microsoft Defender Antivirus изключения.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c8bf5-107">За подробности вижте Конфигуриране [и проверка на изключения за Microsoft Defender Antivirus сканирания](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c8bf5-108">За да избегнете проблеми, [прегледайте Често срещани грешки, за да избегнете при дефиниране на изключения](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c8bf5-109">Не всички правила за ASR поддържат изключения.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c8bf5-110">За да проверите дали вашето правило поддържа изключения, вижте таблицата Правила за намаляване [на повърхността на атака](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c8bf5-111">Правила за намаляване на повърхността на атака</span><span class="sxs-lookup"><span data-stu-id="c8bf5-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c8bf5-112">Повърхността на атаката на вашата организация включва всички места, където хакер може да компрометира организационни устройства или мрежи.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c8bf5-113">Намаляването на повърхността на атаката означава защита на организационните устройства и мрежата, което оставя на хакерите по-малко начини за извършване на атаки.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c8bf5-114">Конфигурирането на правилата за намаляване на повърхността на атаката в Microsoft Defender за крайна точка може да ви помогне.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c8bf5-115">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="c8bf5-115">For more information, see:</span></span>

- [<span data-ttu-id="c8bf5-116">Map ASR правило GUID за име</span><span class="sxs-lookup"><span data-stu-id="c8bf5-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c8bf5-117">Изисквания към правилата за ASR:</span><span class="sxs-lookup"><span data-stu-id="c8bf5-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c8bf5-118">Windows 10 Pro, версия 1709 или по-нова</span><span class="sxs-lookup"><span data-stu-id="c8bf5-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c8bf5-119">Windows 10 Enterprise, версия 1709 или по-нова</span><span class="sxs-lookup"><span data-stu-id="c8bf5-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c8bf5-120">Windows Сървър, версия 1803 (полугодишен канал) или по-нова версия</span><span class="sxs-lookup"><span data-stu-id="c8bf5-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c8bf5-121">Идентифициране на правилното изключване, което да се приложи</span><span class="sxs-lookup"><span data-stu-id="c8bf5-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c8bf5-122">Потърсете eventID 1121 или 1122 в регистрационния файл на Microsoft-Windows-Windows Defender/Операционен.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c8bf5-123">Оценете сценария и контекста на блока и потвърдете, че този сценарий трябва да бъде разблокиран.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c8bf5-124">Прочетете стойността Път в подробните данни за събитието, което е стойността, която дефинира изключението.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c8bf5-125">Направете изключението възможно най-строго.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c8bf5-126">Прилагане на заместващ символ, когато е необходимо (например заместване на променливата потребител).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c8bf5-127">Приложете изключението според нуждите ви от разполагане.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c8bf5-128">За подробности вижте Персонализиране на [правилата за намаляване на повърхността на атаката](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c8bf5-129">Изключването не е зачетено</span><span class="sxs-lookup"><span data-stu-id="c8bf5-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c8bf5-130">Определете дали правилото поддържа изключения.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c8bf5-131">За подробности вижте Правила за [намаляване на повърхността на атака](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c8bf5-132">Прегледайте приложените изключения и проверете с данните за събитието за правописни грешки или неправилно интерпретирани заместващи символи.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c8bf5-133">За повече информация вижте [Поддържани типове изключения](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c8bf5-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c8bf5-134">ако въздействието на правилото е твърде високо, помислете за преместване на правилото (обратно) в режим на проверка, за да извършите по-нататъшно валидиране.</span><span class="sxs-lookup"><span data-stu-id="c8bf5-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c8bf5-135">За подробности вижте Тестване как [функциите на Microsoft Defender за крайна точка работят в режим на проверка.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="c8bf5-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c8bf5-136">Събирайте данни за поддръжка, за да отворите случай на поддръжка, като използвате тази команда:</span><span class="sxs-lookup"><span data-stu-id="c8bf5-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c8bf5-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c8bf5-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c8bf5-138">За повече информация вижте [Проблеми с компютрите за табло към Microsoft Defender за крайни точки](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="c8bf5-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
