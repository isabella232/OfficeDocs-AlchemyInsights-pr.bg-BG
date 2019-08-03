---
title: Проблеми с МВНР
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250154"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="dcd6c-102">Проблеми с МВНР</span><span class="sxs-lookup"><span data-stu-id="dcd6c-102">Issues with MFA</span></span>
<span data-ttu-id="dcd6c-103">Има няколко неща, за да проверите дали потребителите не мога да вляза с помощта на удостоверяване (МВНР)</span><span class="sxs-lookup"><span data-stu-id="dcd6c-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="dcd6c-104">Променения потребител може да бъде блокиран в Azure Active Directory портал.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="dcd6c-105">Ако случаят е такъв, удостоверяване се опитва за това автоматично ще бъдат отказани конкретен потребител.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="dcd6c-106">Моля, следвайте стъпките в тази статия, за да ги деблокирате.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="dcd6c-107">Ако отблокирате потребител не помогне или потребителят не е блокирана можете да опитате да възстановите МВНР за потребителя и те ще преминат през процеса на записвам отново.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="dcd6c-108">Моля, следвайте стъпките в тази статия.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="dcd6c-109">Ако това е първи път разрешен МВРХ и вашите потребители са в състояние да влезете в не-браузъри клиенти като Outlook, Skype и т.н., може би ADAL (Active Directory удостоверяване библиотека) не е разрешена на абонамента си O365.</span><span class="sxs-lookup"><span data-stu-id="dcd6c-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="dcd6c-110">В този случай ще трябва да се свърже с Exchange Online Powershell и да изпълните тази кратка команда:  *комплект-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="dcd6c-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>