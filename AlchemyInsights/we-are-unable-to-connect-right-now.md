---
title: Проблем с активирането – в момента не можем да се свържем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725972"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="82b29-102">Отстраняване на неуспешно свързване на приложенията на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="82b29-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="82b29-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="82b29-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="82b29-104">Проверете защитната стена, антивирусния софтуер и настройките за прокси сървър, за да потвърдите, че не блокират достъпа до интернет за приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="82b29-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="82b29-105">Вижте [диапазони от URL и IP адреси на Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="82b29-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="82b29-106">Отидете на **Старт**  >  **Run**и след това въведете **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="82b29-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="82b29-107">Уверете се, че се изпълняват следните услуги:</span><span class="sxs-lookup"><span data-stu-id="82b29-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="82b29-108">Автоматично настройване на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="82b29-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="82b29-109">Услуга за списък с мрежи</span><span class="sxs-lookup"><span data-stu-id="82b29-109">Network List Service</span></span>
    - <span data-ttu-id="82b29-110">Информиране за местоположения в мрежата</span><span class="sxs-lookup"><span data-stu-id="82b29-110">Network Location Awareness</span></span>
    - <span data-ttu-id="82b29-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="82b29-111">Windows Event Log</span></span>

<span data-ttu-id="82b29-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="82b29-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="82b29-113">Ако имате проблем при стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="82b29-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="82b29-114">**SFC за разлагане**</span><span class="sxs-lookup"><span data-stu-id="82b29-114">**sfc /scannow**</span></span>

<span data-ttu-id="82b29-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="82b29-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="82b29-116">За по-подробна информация вижте ["за съжаление не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка, когато активирате Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="82b29-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>