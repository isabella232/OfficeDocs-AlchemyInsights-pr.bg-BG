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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579926"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="3d558-102">Коригиране на Microsoft 365 приложения "Съжаляваме, друг акаунт от вашата организация вече е влязъл" съобщение</span><span class="sxs-lookup"><span data-stu-id="3d558-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="3d558-103">За да коригирате грешката, използвайте стъпките по-долу:</span><span class="sxs-lookup"><span data-stu-id="3d558-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3d558-104">Премахнете всички служебни акаунти, с изключение на засегнатия акаунт, като използвате настройки на Windows > **Достъп до работа или училище**.</span><span class="sxs-lookup"><span data-stu-id="3d558-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="3d558-105">[Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.</span><span class="sxs-lookup"><span data-stu-id="3d558-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3d558-106">**Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0.</span><span class="sxs-lookup"><span data-stu-id="3d558-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3d558-107">(Напр:\софтуер\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3d558-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3d558-108">Отворете приложение на Office, изберете **Излизане**от  >  **акаунт**  >  **за**файл . След това влезте с потребителски акаунт с валиден лиценз.</span><span class="sxs-lookup"><span data-stu-id="3d558-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="3d558-109">За подробна информация вж. [Акаунти в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3d558-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3d558-110">За Mac вж. [Не можете да влезете в приложение на Office 2016 за Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="3d558-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="3d558-111">За повече информация вижте ["За съжаление друг акаунт от вашата организация е вече влезли в този компютър" в Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="3d558-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>