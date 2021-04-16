---
title: Възникна грешка при проверка на грешката в маркера за достъп по време на настолната версия на Analytics на борда
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813677"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="a2b4c-102">Грешка "Възникна грешка при проверка на маркера за достъп" по време на таблото на Настолните анализи</span><span class="sxs-lookup"><span data-stu-id="a2b4c-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="a2b4c-103">Тази грешка обикновено се наблюдава, когато маркерът за удостоверяване изтече.</span><span class="sxs-lookup"><span data-stu-id="a2b4c-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="a2b4c-104">Обикновено обновяването на страницата обновява маркера.</span><span class="sxs-lookup"><span data-stu-id="a2b4c-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="a2b4c-105">Този проблем обаче може да продължи, ако има правила за условен достъп, приложени към акаунта, който се използва за настолни анализи на компютъра.</span><span class="sxs-lookup"><span data-stu-id="a2b4c-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="a2b4c-106">Можете да прегледате регистрационните файлове за влизане в Azure AD в портала на Azure, за да видите дали има грешки при влизане за акаунта, който се използва за настолни анализи.</span><span class="sxs-lookup"><span data-stu-id="a2b4c-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="a2b4c-107">За повече информация относно условен достъп посетете Планиране [на разполагането на вашия условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="a2b4c-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>