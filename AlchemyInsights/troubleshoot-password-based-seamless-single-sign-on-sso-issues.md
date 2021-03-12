---
title: Отстраняване на проблеми с базирано на парола безпроблемно с еднократна идентификация (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714679"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="983e8-102">Отстраняване на проблеми с базирано на парола безпроблемно с еднократна идентификация (SSO)</span><span class="sxs-lookup"><span data-stu-id="983e8-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="983e8-103">За да научите основите на базиран на парола SSO, вижте [удостоверяване, базирано на парола с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="983e8-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="983e8-104">**Конфигуриране на базиран на парола SSO**</span><span class="sxs-lookup"><span data-stu-id="983e8-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="983e8-105">[Конфигуриране на базирани на парола еднократна идентификация](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -тази статия влиза в повече подробности за ОПЦИЯТА за SSO, базирана на парола.</span><span class="sxs-lookup"><span data-stu-id="983e8-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="983e8-106">Ако приложението, което добавяте, изисква конфигурация по избор и трябва да използвате базирани на парола SSO, тази статия е за вас.</span><span class="sxs-lookup"><span data-stu-id="983e8-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="983e8-107">[Конфигуриране на базиран на парола еднократна идентификация за приложения на по-ниска база](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – прокси сървър на приложението поддържа няколко режима на еднократна идентификация.</span><span class="sxs-lookup"><span data-stu-id="983e8-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="983e8-108">Базираното на парола влизане е предназначено за приложения, които използват комбинация от потребителско име и парола за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="983e8-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="983e8-109">Когато конфигурирате влизане чрез парола за вашето приложение, вашите потребители трябва да влязат в локалното приложение еднократно.</span><span class="sxs-lookup"><span data-stu-id="983e8-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="983e8-110">След това Azure Active Directory съхранява информацията за влизане и автоматично го предоставя на приложението, когато вашите потребители имат достъп до тях отдалечено.</span><span class="sxs-lookup"><span data-stu-id="983e8-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="983e8-111">Би трябвало вече да сте публикували и тествали приложението си чрез прокси сървър за приложения.</span><span class="sxs-lookup"><span data-stu-id="983e8-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="983e8-112">Ако не е, следвайте стъпките в [публикуване на приложения чрез прокси сървър за приложения на AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) и след това продължете конфигурацията на базирани на парола SSO за приложения на по-програми.</span><span class="sxs-lookup"><span data-stu-id="983e8-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="983e8-113">За да отстраните базиран на парола SSO, вижте [отстраняване на неизправности при еднократна идентификация на базата на парола в AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="983e8-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
