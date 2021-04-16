---
title: Проблем с активирането – в момента не можем да се свържем
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806431"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="f677e-102">Коригиране на съобщението "Не можем да се свържем в момента" на приложенията на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f677e-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="f677e-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="f677e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f677e-104">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че не блокират достъпа до интернет до приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f677e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f677e-105">Вижте [Диапазони от URL и IP адреси на Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f677e-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f677e-106">Отидете на **Стартиране**  >  **на изпълнение** и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="f677e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f677e-107">Уверете се, че всички услуги по-долу се изпълняват:</span><span class="sxs-lookup"><span data-stu-id="f677e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f677e-108">Автоматична настройка на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="f677e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f677e-109">Услуга "Списък на мрежата"</span><span class="sxs-lookup"><span data-stu-id="f677e-109">Network List Service</span></span>
    - <span data-ttu-id="f677e-110">Информираност за местоположението на мрежата</span><span class="sxs-lookup"><span data-stu-id="f677e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f677e-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="f677e-111">Windows Event Log</span></span>

<span data-ttu-id="f677e-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="f677e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f677e-113">Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="f677e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f677e-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="f677e-114">**sfc /scannow**</span></span>

<span data-ttu-id="f677e-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="f677e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f677e-116">За подробна информация вижте ["За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно" грешка, когато активирате Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f677e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>