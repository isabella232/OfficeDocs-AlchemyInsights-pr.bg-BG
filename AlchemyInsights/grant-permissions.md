---
title: Даване на разрешения
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900837"
---
# <a name="grant-permissions"></a><span data-ttu-id="81045-102">Даване на разрешения</span><span class="sxs-lookup"><span data-stu-id="81045-102">Grant permissions</span></span>

1. <span data-ttu-id="81045-103">**Предоставяне на разрешение на администратор на клиент**: вижте [даване на разрешение на администратор на клиент за кандидатстване](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) за подробни инструкции за даване на разрешение на администратор на клиент, в портала на AZURE, чрез Azure ad PowerShell или чрез подкана за съгласие.</span><span class="sxs-lookup"><span data-stu-id="81045-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="81045-104">**Даване на съгласие от името на конкретен потребител**: вместо да давате съгласие за цялата организация, администраторът може също да използва [API за Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) , за да даде съгласие за делегирани разрешения от името на един потребител.</span><span class="sxs-lookup"><span data-stu-id="81045-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="81045-105">За повече информация вижте [получаване на достъп от името на потребител](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="81045-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>