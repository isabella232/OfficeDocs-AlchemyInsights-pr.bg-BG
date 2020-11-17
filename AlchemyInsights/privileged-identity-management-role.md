---
title: Поверителна роля за управление на самоличността
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088516"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="5bcbb-102">Привилегирована роля за управление на самоличността (PIM)</span><span class="sxs-lookup"><span data-stu-id="5bcbb-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="5bcbb-103">**Не се разрешават разрешения след активирането на роля**</span><span class="sxs-lookup"><span data-stu-id="5bcbb-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="5bcbb-104">Когато активирате роля в Azure AD поверително управление на самоличността (PIM), активирането може да не се разпространи незабавно във всички портали, които изискват привилегирована роля.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="5bcbb-105">Понякога дори ако промяната е размножена, уеб кеширането в портал може да доведе до това, че промяната не влиза в сила незабавно.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="5bcbb-106">Ако активирането ви е отложено, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="5bcbb-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5bcbb-107">Излезте от портала на Azure и след това влезте отново.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="5bcbb-108">Когато активирате РЕКЛАМНА роля на Azure или ресурсна роля на Azure, ще видите етапите на активирането.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="5bcbb-109">След като сте завършили всички етапи, ще видите връзката "излизане".</span><span class="sxs-lookup"><span data-stu-id="5bcbb-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="5bcbb-110">Можете да използвате тази връзка, за да излезете. Това ще реши повечето случаи за забавяне на активирането.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="5bcbb-111">В PIM Проверете дали сте включени в списъка като член на ролята.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="5bcbb-112">Ако активирате ролята на администратор на Exchange, трябва да излезете и да влезете отново.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="5bcbb-113">Ако проблемът продължава, отворете билет за поддръжка и го отгледате като проблем.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="5bcbb-114">Ако използвате своята роля на администратор на Exchange, за да получите достъп до центъра за сигурност и съответствие, Вижте следващата стъпка.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="5bcbb-115">Ако активирате роля за достъп до центъра за защита и съответствие или ако активирате ролята на администратор на SharePoint, ще получите известно закъснение при активирането от няколко минути до няколко часа.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="5bcbb-116">Това е известен проблем и активно работим с тези екипи, за да отстраним този проблем възможно най-скоро.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="5bcbb-117">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="5bcbb-117">For more information, see:</span></span>

- [<span data-ttu-id="5bcbb-118">Активиране на моите Azure AD роли в PIM</span><span class="sxs-lookup"><span data-stu-id="5bcbb-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="5bcbb-119">Активиране на моите Azure ресурси роли в PIM</span><span class="sxs-lookup"><span data-stu-id="5bcbb-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="5bcbb-120">**Разрешенията не се премахват, след като дезактивират роля или срокът на активиране на роля изтича**</span><span class="sxs-lookup"><span data-stu-id="5bcbb-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="5bcbb-121">Когато дезактивирате роля в Azure AD поверително управление на самоличността или когато изтече срокът на активиране на роля, е възможно да има забавяне там, където можете да продължите да имате достъп.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="5bcbb-122">Ако дезактивирането ви е отложено, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="5bcbb-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5bcbb-123">Ако дезактивирате ролята на администратор на Exchange или срокът на активиране на роля изтича и забелязвате значително забавяне, преди да бъдат премахнати разрешенията, отворете билет за поддръжка и кажете на вашия инженер по поддръжката да ви помогне да подадете билет за този проблем с привилегирования екип за управление на достъпа (PAM).</span><span class="sxs-lookup"><span data-stu-id="5bcbb-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="5bcbb-124">Ако срокът за активиране е изтекъл, но все още имате отворена сесия на браузъра, затворете браузъра си.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="5bcbb-125">Можете да продължите да използвате ролята, докато затворите тази сесия.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="5bcbb-126">Това е известен проблем и разглеждаме потенциална корекция за активно отменяне на всяка сесия, след като активирането изтече.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="5bcbb-127">Ако закъснението ви е различно от тези два сценария, моля, отворете билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="5bcbb-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
