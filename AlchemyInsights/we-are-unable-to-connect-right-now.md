---
title: Проблем при активиране - Не можем да се свържем точно сега
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716161"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="d682b-102">Определяне на office приложения "Не можем да се свържете в момента" съобщение</span><span class="sxs-lookup"><span data-stu-id="d682b-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="d682b-103">Ако се появи това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="d682b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d682b-104">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те не блокират достъпа до интернет за приложенията на Office.</span><span class="sxs-lookup"><span data-stu-id="d682b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="d682b-105">Вижте [url адреси те на Microsoft и ip адреси.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="d682b-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d682b-106">Отидете на **Стартиране на** > **изпълнение**и след това въведете **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="d682b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d682b-107">Уверете се, че са всички следните услуги:</span><span class="sxs-lookup"><span data-stu-id="d682b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d682b-108">Автоматична настройка на свързаните с мрежата устройства</span><span class="sxs-lookup"><span data-stu-id="d682b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d682b-109">Услуга за мрежов списък</span><span class="sxs-lookup"><span data-stu-id="d682b-109">Network List Service</span></span>
    - <span data-ttu-id="d682b-110">Информираност за местоположението в мрежата</span><span class="sxs-lookup"><span data-stu-id="d682b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d682b-111">Регистър на събитията на Windows</span><span class="sxs-lookup"><span data-stu-id="d682b-111">Windows Event Log</span></span>

<span data-ttu-id="d682b-112">Ако една от тези услуги не се изпълнява, опитайте да я стартирате.</span><span class="sxs-lookup"><span data-stu-id="d682b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d682b-113">Ако имате проблем с стартирането на услугата, изпълнете следната команда, като отворите командния ред с повишени разрешения:</span><span class="sxs-lookup"><span data-stu-id="d682b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d682b-114">**SFC /сканиране**</span><span class="sxs-lookup"><span data-stu-id="d682b-114">**sfc /scannow**</span></span>

<span data-ttu-id="d682b-115">След като тази команда приключи, рестартирайте компютъра.</span><span class="sxs-lookup"><span data-stu-id="d682b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d682b-116">За подробна информация вижте ["Съжаляваме, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"грешка при активиране на Office от Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="d682b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>