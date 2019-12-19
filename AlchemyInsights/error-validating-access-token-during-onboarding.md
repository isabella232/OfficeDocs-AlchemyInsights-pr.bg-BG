---
title: Възникна грешка при потвърждаване на грешка при достъп до маркера по време на качването на работния плот
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741118"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="733e5-102">"Възникна грешка при проверка на маркера за достъп" грешка при внедряване на работния плот Analytics</span><span class="sxs-lookup"><span data-stu-id="733e5-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="733e5-103">Тази грешка обикновено се наблюдава при изтичане на маркера за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="733e5-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="733e5-104">Обикновено опресняване на страницата обновява маркера.</span><span class="sxs-lookup"><span data-stu-id="733e5-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="733e5-105">Обаче този проблем може да продължи, ако има някакви правила за условен достъп, приложени към акаунта се използва за настолни компютри анализ.</span><span class="sxs-lookup"><span data-stu-id="733e5-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="733e5-106">Можете да прегледате Azure AD влизане регистрационни файлове в Azure портала да видите дали има грешки при влизане за акаунт се използва за обслужване на работния плот анализ.</span><span class="sxs-lookup"><span data-stu-id="733e5-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="733e5-107">За повече информация относно условен достъп посетете [план вашето разполагане на условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="733e5-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>