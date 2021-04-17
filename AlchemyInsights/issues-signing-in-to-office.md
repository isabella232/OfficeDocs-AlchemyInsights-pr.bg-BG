---
title: Проблеми при влизане в приложения на Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833020"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="60b3d-102">Празен екран за влизане в приложенията на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="60b3d-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="60b3d-103">За да коригирате този проблем, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="60b3d-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="60b3d-104">Инсталирайте най-новите актуализации [за Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="60b3d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="60b3d-105">Нулиране на опциите на Internet Explorer: Отидете на Инструменти Internet  >  **Options**  >  **Advanced**  >  **Reset Internet Explorer Settings** (имайте предвид, че ще загубите настройките по избор) и след това опитайте да влезете отново в Office.</span><span class="sxs-lookup"><span data-stu-id="60b3d-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="60b3d-106">Забраняване на Windows Defender Application Guard (WDAG) или подобна защитна стена или антивирусна програма:</span><span class="sxs-lookup"><span data-stu-id="60b3d-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="60b3d-107">В контролния панел отидете на **Програми и** след това изберете Включване или изключване **на функциите на Windows.**</span><span class="sxs-lookup"><span data-stu-id="60b3d-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="60b3d-108">Ако Windows Defender Application Guard е разрешен, опитайте да го изключите.</span><span class="sxs-lookup"><span data-stu-id="60b3d-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="60b3d-109">**Забележка:** Може да се наложи да рестартирате компютъра.</span><span class="sxs-lookup"><span data-stu-id="60b3d-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="60b3d-110">Уверете се, че добавката Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не се блокира от приложение или защитна стена/антивирусна програма.</span><span class="sxs-lookup"><span data-stu-id="60b3d-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="60b3d-111">[Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="60b3d-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="60b3d-112">**Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0.</span><span class="sxs-lookup"><span data-stu-id="60b3d-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="60b3d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="60b3d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="60b3d-114">За повече информация вижте Проблеми с връзката при влизане след актуализация до [компилация на Office 2016 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="60b3d-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>