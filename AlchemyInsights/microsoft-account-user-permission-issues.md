---
title: Отстраняване на проблем-потребителят не е намерен в директорията
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768790"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="225b3-102">Отстраняване на проблем-потребителят не е намерен в директорията</span><span class="sxs-lookup"><span data-stu-id="225b3-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="225b3-103">Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в директорията, опитайте отново, когато типът на проблема е потребител не в директорията.</span><span class="sxs-lookup"><span data-stu-id="225b3-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="225b3-104">Следните стъпки могат да бъдат завършени за отстраняване на проблема.</span><span class="sxs-lookup"><span data-stu-id="225b3-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="225b3-105">Уверете се, че акаунтът, който е приел имейл поканата е един и същ акаунт, който се използва за влизане по-късно.</span><span class="sxs-lookup"><span data-stu-id="225b3-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="225b3-106">Уверете се, че потребителят използва един и същ акаунт, за да приеме поканата и да подпише в сайта.</span><span class="sxs-lookup"><span data-stu-id="225b3-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="225b3-107">За повече информация вижте [как да управлявате псевдоними за вашия акаунт</a> в Microsoft за управление на Office 365 вход](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="225b3-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="225b3-108">Прегледайте всеки сайт (и), в който потребителят получава грешката.</span><span class="sxs-lookup"><span data-stu-id="225b3-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="225b3-109">Добавете "/_layouts/15/Nari.Six/papripiscupuspusa = 0" (в двойните кавички) до края на URL адреса на сайта</span><span class="sxs-lookup"><span data-stu-id="225b3-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="225b3-110">Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="225b3-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="225b3-111">Изберете потребителя от списъка.</span><span class="sxs-lookup"><span data-stu-id="225b3-111">Select the user from the list.</span></span>

- <span data-ttu-id="225b3-112">Щракнете върху **Премахване на потребителски разрешения** от лентата.</span><span class="sxs-lookup"><span data-stu-id="225b3-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="225b3-113">Добавете обратно потребителя и изпрати поканата на потребителя.</span><span class="sxs-lookup"><span data-stu-id="225b3-113">Add back the User and Resend the invite to the user.</span></span>

