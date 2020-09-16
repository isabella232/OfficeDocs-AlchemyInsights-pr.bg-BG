---
title: Поправяне на приложения на Microsoft 365 Съжаляваме, имаме съобщение за временен проблем със сървъра
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758234"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="d7d55-102">Поправяне на приложенията на Microsoft 365 "за съжаление, имаме съобщение за временен проблем със сървъра"</span><span class="sxs-lookup"><span data-stu-id="d7d55-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="d7d55-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="d7d55-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d7d55-104">Проверете защитната стена, антивирусния софтуер и настройките за прокси сървър, за да потвърдите, че не блокират достъпа до интернет за приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d7d55-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d7d55-105">Вижте [диапазони от URL и IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)адреси.</span><span class="sxs-lookup"><span data-stu-id="d7d55-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d7d55-106">Отидете на **Старт**  >  **Run**и след това въведете **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="d7d55-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d7d55-107">Уверете се, че се изпълняват следните услуги:</span><span class="sxs-lookup"><span data-stu-id="d7d55-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d7d55-108">Автоматично настройване на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="d7d55-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d7d55-109">Услуга за списък с мрежи</span><span class="sxs-lookup"><span data-stu-id="d7d55-109">Network List Service</span></span>
    - <span data-ttu-id="d7d55-110">Информиране за местоположения в мрежата</span><span class="sxs-lookup"><span data-stu-id="d7d55-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d7d55-111">Регистър на събитията в Windows</span><span class="sxs-lookup"><span data-stu-id="d7d55-111">Windows Event Log</span></span>

<span data-ttu-id="d7d55-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="d7d55-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d7d55-113">Ако имате проблем при стартирането на услугата, изпълнете следната команда, като отворите команден прозорец с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="d7d55-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d7d55-114">**SFC за разлагане**</span><span class="sxs-lookup"><span data-stu-id="d7d55-114">**sfc /scannow**</span></span>

<span data-ttu-id="d7d55-115">След като тази команда завърши, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="d7d55-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d7d55-116">За по-подробна информация вижте ["за съжаление не можем да се свържем с вашия акаунт. Моля, опитайте отново по-късно "грешка при активиране](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="d7d55-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>