---
title: 126 Получаването на пощенска кутия не може да бъде намерено за грешка в OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426651"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="c88e3-102">Получаване на пощенска кутия не е намерена грешка в Outlook в уеб?</span><span class="sxs-lookup"><span data-stu-id="c88e3-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="c88e3-103">Ако използвате Outlook в уеб и получите  пощенска кутия, не може да бъде намерена за грешка, акаунтът, който сте използвали за свързване с Outlook в уеб, няма лиценз за Exchange Online и следователно няма пощенска кутия, свързана с акаунта.</span><span class="sxs-lookup"><span data-stu-id="c88e3-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="c88e3-104">Вашият администратор може да присвои лиценз на вашия акаунт, като следва следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="c88e3-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="c88e3-105">Отворете центъра [за администриране на Microsoft 365](https://portal.office.com/adminportal/home#/homepage) и отидете на **Активни** потребители под секцията Потребители и изберете потребителя, който вижда грешката. </span><span class="sxs-lookup"><span data-stu-id="c88e3-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="c88e3-106">На потребителската страница, която  се отваря, отидете на  секцията Лицензи и приложения, изберете съответната стойност за местоположение и дайте лиценз, който съдържа Exchange Online (разгънете лиценза, за да видите подробностите за него).</span><span class="sxs-lookup"><span data-stu-id="c88e3-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="c88e3-107">Когато сте готови, щракнете върху **Запиши промените**.</span><span class="sxs-lookup"><span data-stu-id="c88e3-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="c88e3-108">В някои случаи, ако лицензът вече е присвоен на потребителски акаунт, премахването и повторното присвояване на лиценза помага за разрешаването на проблема и за правилното му осигуряване в системата:</span><span class="sxs-lookup"><span data-stu-id="c88e3-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="c88e3-109">Проверете дали вашите абонаменти за M365 Exchange Online (и други, ако имате такива) са актуални и не са изтекли наскоро.</span><span class="sxs-lookup"><span data-stu-id="c88e3-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="c88e3-110">След като сте се уверили, че абонаментът ви не е изтекъл и на потребителския акаунт е даден валиден лиценз, може да са ви отнели до 24 часа, докато бъде осигурен лицензът, така че може да се наложи да изчакате проблема ви да реши.</span><span class="sxs-lookup"><span data-stu-id="c88e3-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="c88e3-111">За повече информация вижте [Присвояване и управление на лицензи](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="c88e3-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>