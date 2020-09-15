---
title: Проблеми при влизане в приложенията на Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695276"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="4229c-102">Празен екран за влизане в приложенията на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4229c-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="4229c-103">За да коригирате този проблем, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="4229c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="4229c-104">Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="4229c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="4229c-105">Нулиране на опциите **за Internet Explorer: отидете на**  >  **Опции за интернет**за  >  **Разширени**  >  **нулиране на настройките на Internet Explorer** (обърнете внимание, че ще загубите потребителските настройки) и след това опитайте да влезете отново в Office.</span><span class="sxs-lookup"><span data-stu-id="4229c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="4229c-106">Забраняване на приложението за защита на приложения на Windows Defender (WDAG) или подобна защитна стена или антивирусна програма:</span><span class="sxs-lookup"><span data-stu-id="4229c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="4229c-107">В контролния панел отидете на **програми**и след това изберете **включване и изключване на функции на Windows**.</span><span class="sxs-lookup"><span data-stu-id="4229c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="4229c-108">Ако е разрешена защитата на приложения на Windows Defender, опитайте да я забраните.</span><span class="sxs-lookup"><span data-stu-id="4229c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="4229c-109">**Забележка:** Може да се наложи да рестартирате компютъра.</span><span class="sxs-lookup"><span data-stu-id="4229c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="4229c-110">Уверете се, че добавката Microsoft. пад. BrokerPlugin [в пад за матуритет](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не се блокира от никое приложение или защитна стена/антивирусна програма.</span><span class="sxs-lookup"><span data-stu-id="4229c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="4229c-111">[Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="4229c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="4229c-112">**Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0.</span><span class="sxs-lookup"><span data-stu-id="4229c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4229c-113">(Ех: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="4229c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="4229c-114">За повече информация вижте [проблеми с връзката при влизане, след като сте актуализирали до Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="4229c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>