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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754181"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="9bf6c-102">Отстраняване на проблем-потребителят не е намерен в директорията</span><span class="sxs-lookup"><span data-stu-id="9bf6c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="9bf6c-103">Ако потребителите получават съобщение за грешка "потребителят не може да бъде намерен" в директорията.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="9bf6c-104">Опитайте отново, когато типът на проблема е потребител, който не е в директорията.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="9bf6c-105">Следните стъпки могат да бъдат завършени за отстраняване на проблема.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="9bf6c-106">Уверете се, че акаунтът, който е приел имейл поканата е един и същ акаунт, който се използва за влизане по-късно.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="9bf6c-107">Уверете се, че потребителят използва един и същ акаунт, за да приеме поканата и да подпише в сайта.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="9bf6c-108">За повече информация вижте [как да управлявате псевдоними за вашия акаунт</a> в Microsoft за управление на Office 365 вход](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="9bf6c-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="9bf6c-109">Прегледайте всеки сайт (и), в който потребителят получава грешката.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="9bf6c-110">Добавяне на "/_layouts/15/People.aspx/membershipgroupid членове на групата = 0" (в рамките на двойните кавички) до края на URL адреса на сайта.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="9bf6c-111">Пример: HTTPS://_ \ _ "contoso">. SharePoint. com/_оформления/15/хора. aspx/членове = 0.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="9bf6c-112">Изберете потребителя от списъка.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-112">Select the user from the list.</span></span>

- <span data-ttu-id="9bf6c-113">Щракнете върху **Премахване на потребителски разрешения** от лентата.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="9bf6c-114">Добавете обратно потребителя и изпрати поканата на потребителя.</span><span class="sxs-lookup"><span data-stu-id="9bf6c-114">Add back the User and Resend the invite to the user.</span></span>

