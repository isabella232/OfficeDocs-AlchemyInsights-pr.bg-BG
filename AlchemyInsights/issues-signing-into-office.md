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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938134"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="7233f-102">Проблеми с влизане в офис приложения</span><span class="sxs-lookup"><span data-stu-id="7233f-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="7233f-103">За да поправите влизане в проблеми с офис приложения, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="7233f-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="7233f-104">Премахване на всички сметки на работа, с изключение на засегнатите сметка, използвайки Windows настройки > **достъп до работа или училище**.</span><span class="sxs-lookup"><span data-stu-id="7233f-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="7233f-105">[Ясно Office идентификационни данни](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощта на диспечера на идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="7233f-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7233f-106">**Забележка:** Регистър пътеки за Office 2016 са се променили до 16,0.</span><span class="sxs-lookup"><span data-stu-id="7233f-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7233f-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7233f-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7233f-108">Отворете офис приложение, изберете **файл** > **сметка** > **Знак вън**. След това влезете с потребителски акаунт с валиден лиценз.</span><span class="sxs-lookup"><span data-stu-id="7233f-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="7233f-109">За подробна информация вижте [сметки в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="7233f-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="7233f-110">За Mac Вижте [не влезете в 2016 Office за Mac ап](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="7233f-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="7233f-111">Ако грешки при свързване към Office 365, използвайки Office 2013, разреши модерни удостоверяване за клиент на Office.</span><span class="sxs-lookup"><span data-stu-id="7233f-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="7233f-112">За допълнителна информация вижте:</span><span class="sxs-lookup"><span data-stu-id="7233f-112">For more information, see:</span></span>
- [<span data-ttu-id="7233f-113">Не можете да влезете Office 365, Azure или Intune</span><span class="sxs-lookup"><span data-stu-id="7233f-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="7233f-114">Проблеми с връзката в вход след актуализация на Office 2016 изгради 16.0.7967 на Windows 10</span><span class="sxs-lookup"><span data-stu-id="7233f-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="7233f-115">"Съжалявам, друг акаунт от вашата организация е вече влезли в този компютър" в Office</span><span class="sxs-lookup"><span data-stu-id="7233f-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="7233f-116">Отстраняване на вход въпроси с модерни удостоверяване на Office, когато използвате ADFS</span><span class="sxs-lookup"><span data-stu-id="7233f-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)