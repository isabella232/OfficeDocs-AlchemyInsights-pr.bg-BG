---
title: Регистрационни файлове с пароли
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523610"
---
# <a name="password-logs"></a><span data-ttu-id="c4b1e-102">Регистрационни файлове с пароли</span><span class="sxs-lookup"><span data-stu-id="c4b1e-102">Password logs</span></span>

<span data-ttu-id="c4b1e-103">**Имам проблеми при достъп до регистрационни файлове за проверка на нулиране на пароли**</span><span class="sxs-lookup"><span data-stu-id="c4b1e-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="c4b1e-104">За отстраняване на проблеми, свързани с достъпа до регистрите за проверка на нулиране на пароли, изпълнете следната стъпка:</span><span class="sxs-lookup"><span data-stu-id="c4b1e-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="c4b1e-105">Уверете се, че сте упълномощени да преглеждате регистрационни файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="c4b1e-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="c4b1e-106">Разрешават се само следните роли:</span><span class="sxs-lookup"><span data-stu-id="c4b1e-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="c4b1e-107">Глобален администратор</span><span class="sxs-lookup"><span data-stu-id="c4b1e-107">Global administrator</span></span>
 - <span data-ttu-id="c4b1e-108">Администратор по защитата</span><span class="sxs-lookup"><span data-stu-id="c4b1e-108">Security administrator</span></span>
 - <span data-ttu-id="c4b1e-109">Четец за защита</span><span class="sxs-lookup"><span data-stu-id="c4b1e-109">Security reader</span></span>

<span data-ttu-id="c4b1e-110">**Искам да видя всички събития за проверка на нулирането на пароли от момента на първоначалното разполагане**</span><span class="sxs-lookup"><span data-stu-id="c4b1e-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="c4b1e-111">Събития за нулиране на паролата/регистрация на 120 000 се съхраняват в отчетите на последните 30 дни.</span><span class="sxs-lookup"><span data-stu-id="c4b1e-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="c4b1e-112">Това максимално ограничение се отнася за потребителския интерфейс при изтегляне на CSV файла.</span><span class="sxs-lookup"><span data-stu-id="c4b1e-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="c4b1e-113">събития за 1 000 000 са достъпни чрез PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c4b1e-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="c4b1e-114">За повече информация вижте връзките по-долу:</span><span class="sxs-lookup"><span data-stu-id="c4b1e-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="c4b1e-115">Събития за самостоятелно нулиране на пароли от отчетите на Azure AD и API за събития</span><span class="sxs-lookup"><span data-stu-id="c4b1e-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c4b1e-116">Как да изтеглите бързо събития за регистрация на нулиране на пароли с PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4b1e-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="c4b1e-117">**Искам да разбера повече за възможностите за отчитане на нулиране на пароли**</span><span class="sxs-lookup"><span data-stu-id="c4b1e-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="c4b1e-118">Проверете кой е регистрирал или нулирал паролите с регистрационни файлове за проверка на парола на Azure AD в портала на Azure под **потребители и групи**.</span><span class="sxs-lookup"><span data-stu-id="c4b1e-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="c4b1e-119">За повече информация вижте следните връзки:</span><span class="sxs-lookup"><span data-stu-id="c4b1e-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="c4b1e-120">Обзор на отчетите за нулиране на паролата</span><span class="sxs-lookup"><span data-stu-id="c4b1e-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c4b1e-121">Как да преглеждате отчетите за нулиране на паролата в портала на Azure</span><span class="sxs-lookup"><span data-stu-id="c4b1e-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c4b1e-122">Събития за самостоятелно нулиране на пароли от отчетите на Azure AD и API за събития</span><span class="sxs-lookup"><span data-stu-id="c4b1e-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c4b1e-123">Как да изтеглите бързо събития за регистрация на нулиране на пароли с PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4b1e-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


