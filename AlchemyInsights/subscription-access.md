---
title: Достъп за абонамент
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807187"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="0cc88-102">Не можете да влезете в Azure поради проблеми с браузъра (браузърът увисва, запазва завъртането, не се зарежда и т. н.)</span><span class="sxs-lookup"><span data-stu-id="0cc88-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="0cc88-103">Може да ви е повлияна от прекъсване.</span><span class="sxs-lookup"><span data-stu-id="0cc88-103">You might be impacted by an outage.</span></span> <span data-ttu-id="0cc88-104">Проверете дали има текущо прекъсване: [здравен статус на Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="0cc88-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="0cc88-105">Моля, излезте от всички активни сесии на Azure.</span><span class="sxs-lookup"><span data-stu-id="0cc88-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="0cc88-106">Стартирайте уеб браузър по-личен или инкогнито.</span><span class="sxs-lookup"><span data-stu-id="0cc88-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="0cc88-107">Можете също да се опитате да обновите браузъра, да използвате друг браузър, да изтривате бисквитки от кеша, ако по-горе не работи.</span><span class="sxs-lookup"><span data-stu-id="0cc88-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="0cc88-108">Научете повече: [отстраняване на проблеми при влизане](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="0cc88-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="0cc88-109">**Не можете да получите достъп до абонаменти**</span><span class="sxs-lookup"><span data-stu-id="0cc88-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="0cc88-110">В [портала на Azure](https://portal.azure.com/)се уверете, че е избрано правилното Azure Directory от акаунта в горния десен ъгъл.</span><span class="sxs-lookup"><span data-stu-id="0cc88-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="0cc88-111">Уверете се, че в [центъра за акаунти на Azure](https://account.windowsazure.com/Subscriptions)е използван акаунтът.</span><span class="sxs-lookup"><span data-stu-id="0cc88-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="0cc88-112">Научете повече: [отстраняване на неизправности не са намерени абонаменти](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="0cc88-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="0cc88-113">**Не можете да получите достъп до хронологията на фактуриране**</span><span class="sxs-lookup"><span data-stu-id="0cc88-113">**Unable to access billing history**</span></span>

<span data-ttu-id="0cc88-114">Администраторът на акаунта трябва да се увери, че потребителят, който има достъп до информацията за фактуриране, ще бъде добавен в Azure Active Directory като гост потребител: [Добавяне или изтриване на нов потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0cc88-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0cc88-115">След това потребителят трябва да получи роля на глобален администратор: [Присвояване на роля на потребители](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0cc88-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0cc88-116">Публикувай това, потребителят може да получи достъп за плащане чрез правилата за RBAC: [предоставяне на достъп до фактурите](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0cc88-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0cc88-117">**Препоръчвани документи**</span><span class="sxs-lookup"><span data-stu-id="0cc88-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="0cc88-118">Не мога да вляза, за да управлявам абонамента си за Azure</span><span class="sxs-lookup"><span data-stu-id="0cc88-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)