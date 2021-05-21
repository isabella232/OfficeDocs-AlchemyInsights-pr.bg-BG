---
title: Конфигуриране на изключения за Microsoft Defender ATP сканиране
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543674"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="c12d9-102">Конфигуриране на изключения за Microsoft Defender ATP сканиране</span><span class="sxs-lookup"><span data-stu-id="c12d9-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="c12d9-103">По принцип можете да изключите определени файлови разширения и местоположения на папки от Microsoft Defender ATP сканирания.</span><span class="sxs-lookup"><span data-stu-id="c12d9-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="c12d9-104">Можете също да конфигурирате изключения за файлове, отворени от определени процеси.</span><span class="sxs-lookup"><span data-stu-id="c12d9-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="c12d9-105">За повече информация вижте Конфигуриране и [проверка](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) на изключения въз основа на разширението на файла и местоположението на папките и Конфигуриране на изключения [за файлове, отворени от процеси.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c12d9-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="c12d9-106">За да конфигурирате изключения **за Windows Server 2016 и 2019**, вижте [Конфигуриране Microsoft Defender Antivirus изключения на Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="c12d9-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c12d9-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="c12d9-107">**Mac**</span></span>

<span data-ttu-id="c12d9-108">За подробности относно поддържаните типове изключения и конфигурирането на [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) списък с изключения за Mac вижте Поддържани типове изключения и Как да [конфигурирате списъка с изключения](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="c12d9-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="c12d9-109">**Забележка** Можете също да проверите списъците с изключения с помощта на тестовия файл на EICAR.</span><span class="sxs-lookup"><span data-stu-id="c12d9-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="c12d9-110">За повече информация вижте Проверка [на списъците с изключения с тестов файл на EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="c12d9-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="c12d9-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="c12d9-111">**Linux**</span></span>

<span data-ttu-id="c12d9-112">За подробности относно поддържаните типове изключения и конфигурирането на [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) списък с изключения за Linux вижте Поддържани типове изключения и Конфигуриране и проверка на [изключенията за Microsoft Defender ATP за Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="c12d9-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="c12d9-113">**Забележка** Можете също да проверите списъците с изключения с помощта на тестовия файл на EICAR.</span><span class="sxs-lookup"><span data-stu-id="c12d9-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="c12d9-114">За повече информация вижте Проверка [на списъците с изключения с тестов файл на EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="c12d9-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 