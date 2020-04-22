---
title: Коригиране на office приложения за съжаление, имаме временни сървър проблеми съобщение
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764106"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a9791-102">Коригиране на office приложения "За съжаление, имаме временни сървър проблеми"</span><span class="sxs-lookup"><span data-stu-id="a9791-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a9791-103">Ако се появи това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="a9791-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a9791-104">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те не блокират достъпа до интернет за приложенията на Office.</span><span class="sxs-lookup"><span data-stu-id="a9791-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="a9791-105">Вижте [URL адреси и ip адреси.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="a9791-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a9791-106">Отидете на **Стартиране на** > **изпълнение**и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="a9791-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a9791-107">Уверете се, че са всички следните услуги:</span><span class="sxs-lookup"><span data-stu-id="a9791-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a9791-108">Автоматична настройка на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="a9791-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a9791-109">Услуга за мрежов списък</span><span class="sxs-lookup"><span data-stu-id="a9791-109">Network List Service</span></span>
    - <span data-ttu-id="a9791-110">Информираност за местоположението в мрежата</span><span class="sxs-lookup"><span data-stu-id="a9791-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a9791-111">Регистър на събитията на Windows</span><span class="sxs-lookup"><span data-stu-id="a9791-111">Windows Event Log</span></span>

<span data-ttu-id="a9791-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="a9791-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a9791-113">Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="a9791-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a9791-114">**SFC /сканиране**</span><span class="sxs-lookup"><span data-stu-id="a9791-114">**sfc /scannow**</span></span>

<span data-ttu-id="a9791-115">След като тази команда приключи, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="a9791-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a9791-116">За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"грешка при активиране](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a9791-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>