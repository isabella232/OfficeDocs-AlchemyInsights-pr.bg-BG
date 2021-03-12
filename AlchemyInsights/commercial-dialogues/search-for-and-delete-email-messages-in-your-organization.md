---
title: Търсене и изтриване на имейл съобщения във вашата организация
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743777"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="580b2-102">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="580b2-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="580b2-103">Изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="580b2-103">Follow these steps:</span></span>

1. <span data-ttu-id="580b2-104">Ако не сте глобален администратор, за да търсите съобщения, Вашият акаунт трябва да бъде добавен към **ролевата група "Диспечер на откриване** на електронни данни" или към **ролята за управление на търсенето в съответствие**.</span><span class="sxs-lookup"><span data-stu-id="580b2-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="580b2-105">За да изтриете съобщения, ще трябва да се присъедините към **ролевата група за управление на организацията** или към **ролята за управление на търсенето и изчистването**.</span><span class="sxs-lookup"><span data-stu-id="580b2-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="580b2-106">Разрешенията за тези роли се присвояват в [центъра за съответствие на & за защита.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="580b2-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="580b2-107">[Създаване на търсене на съдържание](https://docs.microsoft.com/office365/securitycompliance/content-search) , за да се намери съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="580b2-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="580b2-108">[Свързване към центъра за администриране на & на съвместимост на PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="580b2-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="580b2-109">Ако използвате многофакторно удостоверяване, вижте следните инструкции: [Свързване към центъра за сигурност &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="580b2-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="580b2-110">Изтрийте съобщението: изпълнете `New-ComplianceSearchAction` кратката команда, за да изтриете съобщението.</span><span class="sxs-lookup"><span data-stu-id="580b2-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="580b2-111">Изтритите съобщения се преместват в папката "Възстановими елементи" на потребителя.</span><span class="sxs-lookup"><span data-stu-id="580b2-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="580b2-112">За примерна команда вижте [стъпка 3: Изтрийте съобщението.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="580b2-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
