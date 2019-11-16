---
title: Проблеми с МФП
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768826"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="6f3ab-102">Проблеми с Azure МФП</span><span class="sxs-lookup"><span data-stu-id="6f3ab-102">Issues with Azure MFA</span></span>
<span data-ttu-id="6f3ab-103">Има няколко неща, за да проверите дали потребителите не могат да влязат с помощта на многофакторно удостоверяване (МФП)</span><span class="sxs-lookup"><span data-stu-id="6f3ab-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="6f3ab-104">Засегнатите потребител може да бъде блокиран в Azure Active Directory портал.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="6f3ab-105">Ако това е така, опитите за удостоверяване за този конкретен потребител ще бъдат автоматично отказани.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="6f3ab-106">Следвайте стъпките в тази статия, за да ги деблокирате.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="6f3ab-107">Ако деблокирането на потребителя не помогна или потребителят не е блокиран, можете да опитате да нулирате МФП за потребителя и те ще мине през процеса на записване отново.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="6f3ab-108">Моля, следвайте стъпките в тази статия.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="6f3ab-109">Ако това е първият път, когато сте разрешили МФП и вашите потребители са в състояние да влезете в не-браузъри клиенти като Outlook, Skype и т. н., може би ЛОТАРИНГИЯ (Active Directory удостоверяване библиотека) не е разрешена на вашия абонамент за O365.</span><span class="sxs-lookup"><span data-stu-id="6f3ab-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="6f3ab-110">В този случай ще трябва да се свържете с Exchange Online PowerShell и изпълнете тази команда:  *Set-Организацияconfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="6f3ab-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>