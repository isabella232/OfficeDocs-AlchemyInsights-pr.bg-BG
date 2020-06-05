---
title: Активиране проблем - Ние не сме в състояние да се свържем точно сега
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581864"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="5a897-102">Коригиране на microsoft 365 приложения "Ние не сме в състояние да се свържете в момента" съобщение</span><span class="sxs-lookup"><span data-stu-id="5a897-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="5a897-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="5a897-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="5a897-104">Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да се уверите, че не блокират достъпа до интернет до приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5a897-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="5a897-105">Вижте [URL адресите на Microsoft и диапазоните на IP адресите](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="5a897-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="5a897-106">Отидете в **Старт**  >  **изпълнение**и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="5a897-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="5a897-107">Уверете се, че всички услуги се изпълняват следните:</span><span class="sxs-lookup"><span data-stu-id="5a897-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="5a897-108">Автоматично настройване на свързани в мрежа устройства</span><span class="sxs-lookup"><span data-stu-id="5a897-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="5a897-109">Услуга за списък на мрежи</span><span class="sxs-lookup"><span data-stu-id="5a897-109">Network List Service</span></span>
    - <span data-ttu-id="5a897-110">Осведоменост за местоположението на мрежата</span><span class="sxs-lookup"><span data-stu-id="5a897-110">Network Location Awareness</span></span>
    - <span data-ttu-id="5a897-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="5a897-111">Windows Event Log</span></span>

<span data-ttu-id="5a897-112">Ако една от тези услуги не се изпълнява, опитайте да го стартирате.</span><span class="sxs-lookup"><span data-stu-id="5a897-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="5a897-113">Ако имате проблем при стартиране на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="5a897-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="5a897-114">**SFC / сканиране**</span><span class="sxs-lookup"><span data-stu-id="5a897-114">**sfc /scannow**</span></span>

<span data-ttu-id="5a897-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="5a897-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="5a897-116">За подробна информация вижте ["Съжаляваме, не можем да се свържем с профила ви. Опитайте отново по-късно"грешка, когато активирате Office от Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="5a897-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>