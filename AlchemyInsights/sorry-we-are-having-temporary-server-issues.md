---
title: Поправяне на Приложения на Microsoft 365 Съжаляваме, имаме съобщение за временни проблеми със сървъра
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582692"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="f7412-102">Коригиране на Microsoft 365 приложения "Съжаляваме, имаме временни проблеми със сървъра" съобщение</span><span class="sxs-lookup"><span data-stu-id="f7412-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="f7412-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="f7412-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f7412-104">Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да се уверите, че не блокират достъпа до интернет до приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f7412-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f7412-105">Вижте [URL адреси и диапазони на IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f7412-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f7412-106">Отидете в **Старт**  >  **изпълнение**и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="f7412-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f7412-107">Уверете се, че всички услуги се изпълняват следните:</span><span class="sxs-lookup"><span data-stu-id="f7412-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f7412-108">Автоматично настройване на свързани в мрежа устройства</span><span class="sxs-lookup"><span data-stu-id="f7412-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f7412-109">Услуга за списък на мрежи</span><span class="sxs-lookup"><span data-stu-id="f7412-109">Network List Service</span></span>
    - <span data-ttu-id="f7412-110">Осведоменост за местоположението на мрежата</span><span class="sxs-lookup"><span data-stu-id="f7412-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f7412-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="f7412-111">Windows Event Log</span></span>

<span data-ttu-id="f7412-112">Ако една от тези услуги не се изпълнява, опитайте да го стартирате.</span><span class="sxs-lookup"><span data-stu-id="f7412-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f7412-113">Ако имате проблем при стартиране на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="f7412-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f7412-114">**SFC / сканиране**</span><span class="sxs-lookup"><span data-stu-id="f7412-114">**sfc /scannow**</span></span>

<span data-ttu-id="f7412-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="f7412-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f7412-116">За подробна информация вижте ["Съжаляваме, не можем да се свържем с профила ви. Моля, опитайте отново по-късно"грешка при активиране.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="f7412-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>