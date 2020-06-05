---
title: Проблеми при влизане в приложения на Microsoft 365
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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579854"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="cdb90-102">Коригиране на Microsoft 365 приложения "модулът на надеждната платформа на компютъра не функционира правилно"</span><span class="sxs-lookup"><span data-stu-id="cdb90-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="cdb90-103">За да коригирате грешката, използвайте стъпките по-долу:</span><span class="sxs-lookup"><span data-stu-id="cdb90-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="cdb90-104">Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="cdb90-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="cdb90-105">[Изчистване на идентификационни данни за Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="cdb90-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="cdb90-106">**Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0.</span><span class="sxs-lookup"><span data-stu-id="cdb90-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="cdb90-107">(Напр:\софтуер\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="cdb90-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="cdb90-108">Опитайте [процеса](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) на възстановяване на потребителя да поправи грешките на модула за надеждна платформа (TPM).</span><span class="sxs-lookup"><span data-stu-id="cdb90-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="cdb90-109">Задайте EnableADAL = 0, като използвате следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="cdb90-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="cdb90-110">Щракнете с десния бутон върху бутона "Старт" на Windows, изберете **Изпълнение**, въведете **regedit**, след което изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="cdb90-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="cdb90-111">Изберете **Да,** за да позволите на редактора на системния регистър да прави промени в устройството ви.</span><span class="sxs-lookup"><span data-stu-id="cdb90-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="cdb90-112">В редактора на системния регистър добавете DWORD стойност на **EnableADAL** с настройка **0** под HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="cdb90-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="cdb90-113">За повече информация вижте [проблеми с връзката след актуализация за Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="cdb90-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>