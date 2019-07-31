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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938136"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="520a0-102">Определяне на Office приложения "на вашия компютър опекун платформа модулирам е не функционира правилно" съобщението</span><span class="sxs-lookup"><span data-stu-id="520a0-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="520a0-103">За да коригирате тази грешка, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="520a0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="520a0-104">Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="520a0-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="520a0-105">[Ясно Office идентификационни данни](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощта на диспечера на идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="520a0-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="520a0-106">**Забележка:** Регистър пътеки за Office 2016 са се променили до 16,0.</span><span class="sxs-lookup"><span data-stu-id="520a0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="520a0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="520a0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="520a0-108">Опитайте на [потребителя възстановяване процес](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) към прикрепвам модул за надеждна платформа (TPM) повреди.</span><span class="sxs-lookup"><span data-stu-id="520a0-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="520a0-109">Задайте EnableADAL = 0, използвайки следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="520a0-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="520a0-110">С десния бутон върху бутона Старт на Windows, изберете **изпълнение**, въведете **regedit**и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="520a0-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="520a0-111">Изберете **"да"** да се даде възможност на редактора на системния регистър да направите промени в устройството.</span><span class="sxs-lookup"><span data-stu-id="520a0-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="520a0-112">В редактора на системния регистър Добавете DWORD стойност на **EnableADAL** с настройка на **0** под HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="520a0-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="520a0-113">За повече информация вижте [връзката проблеми в вход след актуализация на Office 2016 строя 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="520a0-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>