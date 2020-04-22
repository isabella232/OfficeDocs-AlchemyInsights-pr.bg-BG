---
title: Отстраняване на проблем - Потребителят не е намерен в директорията
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702727"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6748b-102">Отстраняване на проблем - Потребителят не е намерен в директорията</span><span class="sxs-lookup"><span data-stu-id="6748b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6748b-103">Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в директорията, опитайте отново, когато тип на проблема не е в директорията.</span><span class="sxs-lookup"><span data-stu-id="6748b-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6748b-104">Следните стъпки могат да бъдат завършени, за да отстраните проблема.</span><span class="sxs-lookup"><span data-stu-id="6748b-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6748b-105">Уверете се, че акаунтът, който е приел поканата за имейл, е същият, който се използва за влизане в по-късно.</span><span class="sxs-lookup"><span data-stu-id="6748b-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6748b-106">Уверете се, че потребителят използва същия акаунт, за да приеме поканата и влезе в сайта.</span><span class="sxs-lookup"><span data-stu-id="6748b-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6748b-107">За повече информация [вж.</a> ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="6748b-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6748b-108">Намерете всеки сайт(и), в който потребителят получава грешката.</span><span class="sxs-lookup"><span data-stu-id="6748b-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6748b-109">Добавете "/_layouts/15/people.aspx/членска група=0" (в рамките на двойните кавички) към края на URL адреса на сайта.</span><span class="sxs-lookup"><span data-stu-id="6748b-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6748b-110">Пример: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6748b-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6748b-111">Изберете потребителя от списъка.</span><span class="sxs-lookup"><span data-stu-id="6748b-111">Select the user from the list.</span></span>

- <span data-ttu-id="6748b-112">Щракнете върху **Премахване на потребителски разрешения** от лентата.</span><span class="sxs-lookup"><span data-stu-id="6748b-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6748b-113">Добавете обратно потребителя и изпрати покана та на потребителя.</span><span class="sxs-lookup"><span data-stu-id="6748b-113">Add back the User and Resend the invite to the user.</span></span>

