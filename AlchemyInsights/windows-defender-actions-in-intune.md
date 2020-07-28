---
title: Действия на Windows защитника в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438908"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="27b16-102">Действия на Windows защитника в Intune</span><span class="sxs-lookup"><span data-stu-id="27b16-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="27b16-103">Intune може да се използва за задействане на сканиране по заявка и актуализация на сигнатури за вируси за Windows Defender на отделни устройства.</span><span class="sxs-lookup"><span data-stu-id="27b16-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="27b16-104">След успешно задействане на отдалечено действие дейността се отразява в регистрационния файл на Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="27b16-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="27b16-105">Правилата за Защита на Windows Endpoint позволяват създаването на допълнителни настройки за функциите на Windows Defender в Intune и приложени към набори от устройства.</span><span class="sxs-lookup"><span data-stu-id="27b16-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="27b16-106">За повече подробности относно задействането на действия на Windows Защитника вижте [Конфигуриране и изпълнение на сканирани сканирания на Microsoft Defender Antivirus](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus)при поискване .</span><span class="sxs-lookup"><span data-stu-id="27b16-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>