---
title: Проблеми с влизане в офис приложения
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938135"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="94f16-102">Празен екран за вход в офис приложения</span><span class="sxs-lookup"><span data-stu-id="94f16-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="94f16-103">За да коригирате този проблем, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="94f16-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="94f16-104">Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="94f16-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="94f16-105">Начално състояние на Internet Explorer опции: отидете в **инструменти** > **Интернет опции** > **Разширени** > **Нулиране на настройките на Internet Explorer** (имайте предвид, че ще загубите персонализирани настройки) и след това се опитайте влизате отново в офиса.</span><span class="sxs-lookup"><span data-stu-id="94f16-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="94f16-106">Да изключите Windows Defender приложение охрана (WDAG) или друга подобна защитна стена или антивирусна програма:</span><span class="sxs-lookup"><span data-stu-id="94f16-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="94f16-107">В контролния панел преминете към **програми**и след това изберете **въртя Прозорец черта на или на разстояние**.</span><span class="sxs-lookup"><span data-stu-id="94f16-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="94f16-108">Ако Windows Defender приложение гвардия е разрешено, опитайте да го забраните.</span><span class="sxs-lookup"><span data-stu-id="94f16-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="94f16-109">**Забележка:** Може да се наложи да рестартирате компютъра.</span><span class="sxs-lookup"><span data-stu-id="94f16-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="94f16-110">Уверете се, че Microsoft.AAD.BrokerPlugin [Пад WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не е блокиран от всяко приложение или програма за защитна стена и антивирусен.</span><span class="sxs-lookup"><span data-stu-id="94f16-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="94f16-111">[Ясно Office идентификационни данни](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощта на диспечера на идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="94f16-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="94f16-112">**Забележка:** Регистър пътеки за Office 2016 са се променили до 16,0.</span><span class="sxs-lookup"><span data-stu-id="94f16-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="94f16-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="94f16-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="94f16-114">За повече информация вижте [връзката проблеми в вход след актуализация на Office 2016 строя 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="94f16-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>