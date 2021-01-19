---
title: Отстраняване на проблеми с потребителското съгласие
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900838"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="8819f-102">Отстраняване на проблеми с потребителското съгласие</span><span class="sxs-lookup"><span data-stu-id="8819f-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="8819f-103">Можете да конфигурирате как крайните потребители да се съгласяват с приложения през портала на Azure или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8819f-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="8819f-104">Вижте [Настройки на потребителско съгласие](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="8819f-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="8819f-105">Администраторът може също да използва [API за Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , за да даде съгласие за делегираните разрешения от името на един потребител.</span><span class="sxs-lookup"><span data-stu-id="8819f-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="8819f-106">За повече информация вижте [получаване на достъп от името на потребител](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="8819f-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="8819f-107">[Грешки при одобрение на потребители](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): тази статия описва грешки, които могат да възникнат по време на процеса на даване на съгласие на приложение.</span><span class="sxs-lookup"><span data-stu-id="8819f-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="8819f-108">Ако отстранявате проблеми с неочакваното съгласие, които не съдържат съобщения за грешка, вижте [сценарии за удостоверяване за AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="8819f-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>