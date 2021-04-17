---
title: Коригиране на приложения на Microsoft 365 За съжаление, имаме съобщение за временни проблеми със сървъра
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835260"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="9f629-102">Коригиране на приложенията на Microsoft 365 "За съжаление, имаме временни проблеми със сървъра"</span><span class="sxs-lookup"><span data-stu-id="9f629-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="9f629-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="9f629-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9f629-104">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че не блокират достъпа до интернет до приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9f629-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9f629-105">Вижте [ДИАПАЗОНИ на URL адреси и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9f629-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9f629-106">Отидете на **Стартиране**  >  **на изпълнение** и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="9f629-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9f629-107">Уверете се, че всички услуги по-долу се изпълняват:</span><span class="sxs-lookup"><span data-stu-id="9f629-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9f629-108">Автоматична настройка на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="9f629-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9f629-109">Услуга "Списък на мрежата"</span><span class="sxs-lookup"><span data-stu-id="9f629-109">Network List Service</span></span>
    - <span data-ttu-id="9f629-110">Информираност за местоположението на мрежата</span><span class="sxs-lookup"><span data-stu-id="9f629-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9f629-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="9f629-111">Windows Event Log</span></span>

<span data-ttu-id="9f629-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="9f629-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9f629-113">Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="9f629-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9f629-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="9f629-114">**sfc /scannow**</span></span>

<span data-ttu-id="9f629-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="9f629-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9f629-116">За подробна информация вижте ["За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно" грешка, когато активирате](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="9f629-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>