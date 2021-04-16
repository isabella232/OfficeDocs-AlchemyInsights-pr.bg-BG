---
title: Проблеми с многофакторните
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810473"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="b5869-102">Проблеми с MFA на Azure</span><span class="sxs-lookup"><span data-stu-id="b5869-102">Issues with Azure MFA</span></span>
<span data-ttu-id="b5869-103">Има няколко неща, които трябва да проверите дали потребителите не могат да внедлят влизане с помощта на многофакторно удостоверяване (MFA)</span><span class="sxs-lookup"><span data-stu-id="b5869-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b5869-104">Засегнатият потребител може да бъде блокиран в портала на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5869-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b5869-105">Ако случаят е такъв, опитите за удостоверяване за този конкретен потребител ще бъдат автоматично отказани.</span><span class="sxs-lookup"><span data-stu-id="b5869-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b5869-106">Следвайте стъпките в тази статия, за да ги деблокирате.</span><span class="sxs-lookup"><span data-stu-id="b5869-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b5869-107">Ако деблокиране на потребителя не помогне или потребителят не е блокиран, можете да опитате да нулирате MFA за потребителя и те ще преминат през процеса на записване отново.</span><span class="sxs-lookup"><span data-stu-id="b5869-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b5869-108">Следвайте стъпките в тази статия.</span><span class="sxs-lookup"><span data-stu-id="b5869-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b5869-109">Ако това е първият път, когато сте разрешили MFA и вашите потребители не могат да влезят в клиенти, които не са браузъри, като например Outlook, Skype и т.н., може би ADAL (библиотека за удостоверяване на Active Directory) не е разрешена във вашия абонамент за O365.</span><span class="sxs-lookup"><span data-stu-id="b5869-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b5869-110">В този случай ще трябва да се свържете към Powershell на Exchange Online и да изпълните тази кратка команда:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="b5869-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>