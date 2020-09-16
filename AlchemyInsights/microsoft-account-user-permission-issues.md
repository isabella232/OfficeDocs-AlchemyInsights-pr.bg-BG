---
title: Отстраняване на проблема – потребителят не е намерен в указателя
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725396"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ca455-102">Отстраняване на проблема – потребителят не е намерен в указателя</span><span class="sxs-lookup"><span data-stu-id="ca455-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ca455-103">Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в указателя, опитайте отново, където типът на проблема е потребител, който не е в справочния указател.</span><span class="sxs-lookup"><span data-stu-id="ca455-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ca455-104">Можете да изпълните следните стъпки, за да отстраните проблема.</span><span class="sxs-lookup"><span data-stu-id="ca455-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ca455-105">Уверете се, че акаунтът, който е приел поканата за имейл, е същият акаунт, който се използва за влизане по-късно.</span><span class="sxs-lookup"><span data-stu-id="ca455-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ca455-106">Уверете се, че потребителят използва един и същ акаунт, за да приеме поканата и да влезе в сайта.</span><span class="sxs-lookup"><span data-stu-id="ca455-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ca455-107">За повече информация вижте [как да управлявате псевдоними за своя акаунт в Microsoft, </a> за да управлявате Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ca455-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ca455-108">Отидете до всеки сайт (ове), в който потребителят получава грешката.</span><span class="sxs-lookup"><span data-stu-id="ca455-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ca455-109">Добавете "/_layouts/15/People.aspx/membershipgroupid = 0" (в двойните кавички) в края на URL адреса на сайта.</span><span class="sxs-lookup"><span data-stu-id="ca455-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ca455-110">Пример: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ca455-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ca455-111">Изберете потребителя от списъка.</span><span class="sxs-lookup"><span data-stu-id="ca455-111">Select the user from the list.</span></span>

- <span data-ttu-id="ca455-112">Щракнете върху **Премахване на потребителските разрешения** от лентата.</span><span class="sxs-lookup"><span data-stu-id="ca455-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ca455-113">Добавете обратно потребителя и повторно изпратете поканата на потребителя.</span><span class="sxs-lookup"><span data-stu-id="ca455-113">Add back the User and Resend the invite to the user.</span></span>

