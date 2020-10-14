---
title: Внедряване на Win32 приложението
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461741"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="a9687-102">Внедряване на Win32 приложението</span><span class="sxs-lookup"><span data-stu-id="a9687-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="a9687-103">Приложението Microsoft позволява Win32 приложения, включително, но не само MSI и. EXE за разполагане на устройства с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a9687-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="a9687-104">Използваният механизъм за разполагане изисква разширеното разширение за управление (IME) да присъства на целевото устройство.</span><span class="sxs-lookup"><span data-stu-id="a9687-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="a9687-105">IME ще се инсталира автоматично като резултат от насочване на скрипт на PowerShell или разполагане на Win32 към потребител/устройство.</span><span class="sxs-lookup"><span data-stu-id="a9687-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="a9687-106">Има и набор от предварителни изисквания, които трябва да бъдат изпълнени, за да се разположи Win32 приложенията, които включват:</span><span class="sxs-lookup"><span data-stu-id="a9687-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="a9687-107">Поддържани платформи: Windows 10 версия 1607 или по-нова (версии Enterprise, Pro и Education).</span><span class="sxs-lookup"><span data-stu-id="a9687-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="a9687-108">Поддържана архитектура: x86 и x64.</span><span class="sxs-lookup"><span data-stu-id="a9687-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="a9687-109">Управление на устройства: пад присъединен и автоматично записване (включително хибриден домейн, присъединен към и автоматично записване на групови правила).</span><span class="sxs-lookup"><span data-stu-id="a9687-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="a9687-110">Формат на пакета приложения: **intunewin**  файл, подготвен от [инструмента за подготовка на съдържание за Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="a9687-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="a9687-111">Ограничения</span><span class="sxs-lookup"><span data-stu-id="a9687-111">Limitations:</span></span>
    - <span data-ttu-id="a9687-112">Максимален размер: 8GB.</span><span class="sxs-lookup"><span data-stu-id="a9687-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="a9687-113">Неподдържана архитектура: ARMs.</span><span class="sxs-lookup"><span data-stu-id="a9687-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="a9687-114">Прегледайте документа "[Добавяне, даване и следене на приложението Win32 в Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" за информация относно тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="a9687-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="a9687-115">Подробни данни за разполагането на приложения за отстраняване на неизправности в Windows, включително Win32 приложенията, могат да бъдат преглеждани в следните документи</span><span class="sxs-lookup"><span data-stu-id="a9687-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="a9687-116">Отстраняване на проблеми с инсталирането на приложения</span><span class="sxs-lookup"><span data-stu-id="a9687-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="a9687-117">Отстраняване на неизправности при Win32 приложения</span><span class="sxs-lookup"><span data-stu-id="a9687-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)