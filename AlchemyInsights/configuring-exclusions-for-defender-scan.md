---
title: Конфигуриране на изключвания за Microsoft Defender ATP сканиране
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713327"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="e38b8-102">Конфигуриране на изключвания за Microsoft Defender ATP сканиране</span><span class="sxs-lookup"><span data-stu-id="e38b8-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="e38b8-103">В общи линии можете да изключите определени файлови разширения и местоположения на папките от Microsoft Defender ATP сканиране.</span><span class="sxs-lookup"><span data-stu-id="e38b8-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="e38b8-104">Можете също да конфигурирате изключвания за файлове, които са отворени от определени процеси.</span><span class="sxs-lookup"><span data-stu-id="e38b8-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="e38b8-105">За повече информация вижте, [конфигурирайте и проверявайте изключенията на базата на разширението на файла и местоположението на папката](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) и [конфигурирайте изключения за файлове, които са отворени чрез процеси](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="e38b8-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="e38b8-106">За да конфигурирате изключвания за  **Windows server 2016 и 2019**, вижте [Конфигуриране на изключвания на антивирусни програми за Microsoft Defender в Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="e38b8-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="e38b8-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="e38b8-107">**Mac**</span></span>

<span data-ttu-id="e38b8-108">За подробности относно поддържаните типове изключвания и конфигурирането на списък с изключения за Mac Вижте [поддържани типове изключвания](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) и [как да конфигурирате списъка с изключвания](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="e38b8-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="e38b8-109">**Забележка** Можете също да проверите списъците с изключения чрез тестовия файл на EICAR.</span><span class="sxs-lookup"><span data-stu-id="e38b8-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e38b8-110">За повече информация вижте [проверка на списъците с изключения с тестовия файл на eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="e38b8-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="e38b8-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="e38b8-111">**Linux**</span></span>

<span data-ttu-id="e38b8-112">За подробности относно поддържаните типове изключвания и конфигурирането на списък с изключения за Линукс вижте [поддържани типове изключвания](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) и [Конфигуриране и проверка на изключвания за Microsoft Defender ATP за Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="e38b8-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="e38b8-113">**Забележка** Можете също да проверите списъците с изключения чрез тестовия файл на EICAR.</span><span class="sxs-lookup"><span data-stu-id="e38b8-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e38b8-114">За повече информация вижте [проверка на списъците с изключения с тестовия файл на eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="e38b8-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 