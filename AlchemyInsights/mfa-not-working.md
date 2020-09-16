---
title: Проблеми с МВНР
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755120"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="9417b-102">Проблеми с Azure МВНР</span><span class="sxs-lookup"><span data-stu-id="9417b-102">Issues with Azure MFA</span></span>
<span data-ttu-id="9417b-103">Има няколко неща, които трябва да проверите дали потребителите не могат да влизат, като използват многофакторно удостоверяване (МВНР)</span><span class="sxs-lookup"><span data-stu-id="9417b-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="9417b-104">Засегнатите потребители могат да бъдат блокирани в Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="9417b-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="9417b-105">Ако това е така, опитите за удостоверяване за този конкретен потребител ще бъдат отхвърлени автоматично.</span><span class="sxs-lookup"><span data-stu-id="9417b-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="9417b-106">Моля, следвайте стъпките в тази статия, за да ги разблокирате.</span><span class="sxs-lookup"><span data-stu-id="9417b-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="9417b-107">Ако разблокирането на потребителя не е помогнало или потребителят не е блокиран, можете да се опитате да нулирате МВНР за потребителя и той отново ще премине през процеса на записване.</span><span class="sxs-lookup"><span data-stu-id="9417b-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="9417b-108">Моля, следвайте стъпките в тази статия.</span><span class="sxs-lookup"><span data-stu-id="9417b-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="9417b-109">Ако това е първият път, когато сте активирали МВНР и вашите потребители не могат да влязат в клиенти, които не са браузъри, като например Outlook, Skype и т. н., може би ADAL (библиотека за удостоверяване на Active Directory) не е разрешена за вашия абонамент за O365.</span><span class="sxs-lookup"><span data-stu-id="9417b-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="9417b-110">В този случай ще трябва да се свържете с PowerShell на Exchange Online и да изпълните тази кратка команда:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="9417b-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>