---
title: Отстраняване на проблем - потребителят не е намерен в директорията
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249902"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="228f5-102">Отстраняване на проблем - потребителят не е намерен в директорията</span><span class="sxs-lookup"><span data-stu-id="228f5-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="228f5-103">Ако потребителите получават грешка съобщение "потребител не могат да бъдат намерени" в директорията.</span><span class="sxs-lookup"><span data-stu-id="228f5-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="228f5-104">Моля, опитайте отново където изход тип потребител не е в директорията.</span><span class="sxs-lookup"><span data-stu-id="228f5-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="228f5-105">Следните стъпки може да бъде завършена за да отстраните проблема.</span><span class="sxs-lookup"><span data-stu-id="228f5-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="228f5-106">Осигуряване на сметка, която приема имейл покана е една и съща сметка, която се използва за да влезете в по-късно.</span><span class="sxs-lookup"><span data-stu-id="228f5-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="228f5-107">Уверете се, че потребителят използва същата сметка да приемат покани и да влезете в сайта.</span><span class="sxs-lookup"><span data-stu-id="228f5-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="228f5-108">За повече информация, виж [как да управлявате псевдоними за вашия акаунт в Microsoft</a> за управление на Office 365 вход](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="228f5-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="228f5-109">Преминете към всеки сайт (ове), в която потребителят получава грешка.</span><span class="sxs-lookup"><span data-stu-id="228f5-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="228f5-110">Добави "/ _layouts/15/people.aspx/membershipgroupid=0" (в кавички) в края на URL адреса на сайта.</span><span class="sxs-lookup"><span data-stu-id="228f5-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="228f5-111">Пример: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="228f5-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="228f5-112">Изберете потребителя от списъка.</span><span class="sxs-lookup"><span data-stu-id="228f5-112">Select the user from the list.</span></span>

- <span data-ttu-id="228f5-113">Щракнете върху **Премахване на потребителски разрешения** от лентата.</span><span class="sxs-lookup"><span data-stu-id="228f5-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="228f5-114">Добавяне обратно на потребителя и изпрати покани на потребителя.</span><span class="sxs-lookup"><span data-stu-id="228f5-114">Add back the User and Resend the invite to the user.</span></span>

