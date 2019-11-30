---
title: Фиксиране на приложения на Office Съжаляваме, имаме временно съобщение за проблеми със сървъра
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627979"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="3a3a0-102">Определяне на приложенията на Office "Съжаляваме, имаме временен сървър проблеми" съобщение</span><span class="sxs-lookup"><span data-stu-id="3a3a0-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="3a3a0-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="3a3a0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3a3a0-104">Проверете защитната стена, антивирусния софтуер и настройките на прокси сървъра, за да потвърдите, че те не блокират интернет достъпа до приложенията на Office.</span><span class="sxs-lookup"><span data-stu-id="3a3a0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="3a3a0-105">Вижте [URL адресите на Office 365 и IP адресните диапазони](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3a3a0-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="3a3a0-106">Отидете на **Стартирай** > **, след**което въведете **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="3a3a0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="3a3a0-107">Уверете се, че всички следните услуги се изпълняват:</span><span class="sxs-lookup"><span data-stu-id="3a3a0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="3a3a0-108">Автоматична настройка на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="3a3a0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="3a3a0-109">Услуга за мрежови списъци</span><span class="sxs-lookup"><span data-stu-id="3a3a0-109">Network List Service</span></span>
    - <span data-ttu-id="3a3a0-110">Осведоменост за местоположението в мрежата</span><span class="sxs-lookup"><span data-stu-id="3a3a0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="3a3a0-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="3a3a0-111">Windows Event Log</span></span>

<span data-ttu-id="3a3a0-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="3a3a0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="3a3a0-113">Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="3a3a0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="3a3a0-114">**сок/скансега**</span><span class="sxs-lookup"><span data-stu-id="3a3a0-114">**sfc /scannow**</span></span>

<span data-ttu-id="3a3a0-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="3a3a0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="3a3a0-116">За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка при активиране на Office от Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="3a3a0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>