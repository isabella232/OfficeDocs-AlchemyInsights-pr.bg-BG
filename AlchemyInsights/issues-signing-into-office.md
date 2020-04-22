---
title: Проблеми при влизане в приложения на Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762964"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="eb030-102">Проблеми при влизане в приложения на Office</span><span class="sxs-lookup"><span data-stu-id="eb030-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="eb030-103">За да отстраните проблеми с влизането с приложенията на Office, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="eb030-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="eb030-104">Премахнете всички работни акаунти, с изключение на засегнатия акаунт, като използвате Windows Settings > **Достъп до работа или училище**.</span><span class="sxs-lookup"><span data-stu-id="eb030-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="eb030-105">[Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="eb030-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="eb030-106">**Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0.</span><span class="sxs-lookup"><span data-stu-id="eb030-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="eb030-107">(Преди: \Софтуер\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="eb030-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="eb030-108">Отворете приложение на Office, изберете **Изход от файлов** > **акаунт** > **.** След това влезте с потребителски акаунт с валиден лиценз.</span><span class="sxs-lookup"><span data-stu-id="eb030-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="eb030-109">За подробна информация вж. [Акаунти в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="eb030-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="eb030-110">За Mac вж. [Не можете да влезете в приложение на Office 2016 за Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="eb030-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="eb030-111">Ако грешки при свързване към Microsoft 365 с помощта на Office 2013, разрешаване на съвременни удостоверяване за клиент на Office.</span><span class="sxs-lookup"><span data-stu-id="eb030-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="eb030-112">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="eb030-112">For more information, see:</span></span>
- [<span data-ttu-id="eb030-113">Не можете да влезете в Microsoft 365, Azure или Intune</span><span class="sxs-lookup"><span data-stu-id="eb030-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="eb030-114">Проблеми с връзката в влизане след актуализация на Office 2016 компилация 16.0.7967 на Windows 10</span><span class="sxs-lookup"><span data-stu-id="eb030-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="eb030-115">"За съжаление, друг акаунт от вашата организация вече е влязъл в този компютър" в Office</span><span class="sxs-lookup"><span data-stu-id="eb030-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="eb030-116">Отстраняване на проблеми с влизане в Office съвременни удостоверяване, когато използвате ADFS</span><span class="sxs-lookup"><span data-stu-id="eb030-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)