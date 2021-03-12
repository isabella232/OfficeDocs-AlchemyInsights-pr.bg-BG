---
title: Проблеми с инсталирането на Microsoft Defender на Mac или Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713284"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="7540b-102">Проблеми с инсталирането на Microsoft Defender на Mac или Linux</span><span class="sxs-lookup"><span data-stu-id="7540b-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="7540b-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="7540b-103">**Mac**</span></span>

- <span data-ttu-id="7540b-104">Уверете се, че системните изисквания са изпълнени, преди да инсталирате Microsoft Defender ATP for Mac.</span><span class="sxs-lookup"><span data-stu-id="7540b-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="7540b-105">За повече информация вижте [как да инсталирате Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="7540b-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="7540b-106">Прегледайте информацията във файла: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="7540b-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="7540b-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="7540b-107">**Linux**</span></span>

- <span data-ttu-id="7540b-108">Уверете се, че системните изисквания са изпълнени, преди да инсталирате Microsoft Defender ATP за Линукс.</span><span class="sxs-lookup"><span data-stu-id="7540b-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="7540b-109">За повече информация вижте [как да инсталирате Microsoft Defender ATP за Линукс](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="7540b-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="7540b-110">За да се уверите, че услугата MDATP се изпълнява, вижте [Неуспешно инсталиране](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="7540b-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="7540b-111">За отстраняване на неизправности и отстраняване на проблеми Ако услугата не се изпълнява, вижте [стъпки за отстраняване на неизправности, ако услугата mdatp не се изпълнява](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="7540b-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="7540b-112">За стъпки за проверка на конфигурацията на клиента, което проверява изправността на продукта, и за да изпълните тест за откриване в текстов файл на EICAR, вижте [Конфигуриране на клиент](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="7540b-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="7540b-113">**Забележка** За списък на поддържаните файлови системи за дейности в Access вижте [Microsoft Defender ATP за Линукс](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="7540b-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>