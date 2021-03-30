---
title: Проблеми с клиента за регистрация на приложения или проблеми със сертификата
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404214"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="2b543-102">Проблеми с клиента за регистрация на приложения или проблеми със сертификата</span><span class="sxs-lookup"><span data-stu-id="2b543-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="2b543-103">Изтичане на тайната на клиента на приложението?</span><span class="sxs-lookup"><span data-stu-id="2b543-103">Application client secret expiring?</span></span>

<span data-ttu-id="2b543-104">Независимо как е създадено регистрираното приложение, независимо дали чрез стандартния процес на регистрация в портала за регистрация на приложения, или ако директорът на услугата е създаден във вашия клиент с помощта на съгласие за приложение, ще трябва да се създаде нова тайна на клиента преди изтичането на текущия и актуализиран в кода на свързаното приложение.</span><span class="sxs-lookup"><span data-stu-id="2b543-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="2b543-105">Максималният период на валидност е 2 години.</span><span class="sxs-lookup"><span data-stu-id="2b543-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="2b543-106">Като напомняне тайната стойност трябва да бъде записана, тъй като тя повече няма да се вижда, след като напусне страницата "Регистрации на приложения" в портала.</span><span class="sxs-lookup"><span data-stu-id="2b543-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="2b543-107">За повече информация вижте [Бързо започване: Регистриране на приложение в платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) и [Най-добри практики за платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="2b543-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="2b543-108">За да научите повече, вижте [Създаване на приложение azure AD & на услугата в портала – платформа за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="2b543-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
