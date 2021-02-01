---
title: Проблеми с идентификационните данни
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063586"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="7b559-102">Проблеми с идентификационните данни</span><span class="sxs-lookup"><span data-stu-id="7b559-102">Issues with credentials</span></span>

<span data-ttu-id="7b559-103">[Платформата за самоличност на Microsoft и потокът на идентификационните данни за клиент на OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) описват как да програмирате директно спрямо идентификационните данни за клиент на OAuth 2,0 предоставят поток.</span><span class="sxs-lookup"><span data-stu-id="7b559-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="7b559-104">**Как да управлявам паролата или идентификационните данни за сертификата на дадено приложение?**</span><span class="sxs-lookup"><span data-stu-id="7b559-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="7b559-105">В Azure CLI можете да използвате [идентификационни данни за приложенията на приложението](https://docs.microsoft.com/cli/azure/ad/app/credential) , за да изтриете, изведете или нулирате паролата или идентификационните данни за сертификата на дадено приложение.</span><span class="sxs-lookup"><span data-stu-id="7b559-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="7b559-106">**Как моите потребители нулират своите пароли?**</span><span class="sxs-lookup"><span data-stu-id="7b559-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="7b559-107">Потребителите трябва да се [регистрират за самостоятелно нулиране на паролата](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , преди да могат да нулират паролите си.</span><span class="sxs-lookup"><span data-stu-id="7b559-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="7b559-108">След като потребителят е регистрирал, той може да следва инструкциите в тази статия, за да нулира паролата си: [нулиране на вашата служебна или учебна парола](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="7b559-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="7b559-109">**Как потребителите ще сменят паролите си?**</span><span class="sxs-lookup"><span data-stu-id="7b559-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="7b559-110">Потребителите могат да следват стъпките в тази статия, за да променят паролите си: [как да промените паролата си](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="7b559-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="7b559-111">Те също могат да [управляват паролите за приложения за потвърждаване в две стъпки](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="7b559-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="7b559-112">**Потребителят ми получава съобщение за грешка при промяна или нулиране на паролата**</span><span class="sxs-lookup"><span data-stu-id="7b559-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="7b559-113">Тази връзка ще предостави информация за често срещани проблеми, които могат да възникнат, когато потребителят се опитва да нулира паролата си: [често срещани проблеми и техните решения](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="7b559-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="7b559-114">**Имам проблем при нулиране на потребителска парола**</span><span class="sxs-lookup"><span data-stu-id="7b559-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="7b559-115">Уверете се, че имате разрешение за нулиране на пароли.</span><span class="sxs-lookup"><span data-stu-id="7b559-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="7b559-116">*Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.*</span><span class="sxs-lookup"><span data-stu-id="7b559-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7b559-117">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="7b559-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="7b559-118">Уверете се, че разбирате изискванията за лицензиране:</span><span class="sxs-lookup"><span data-stu-id="7b559-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="7b559-119">Трябва да имате поне един лиценз, присвоен във вашата организация:</span><span class="sxs-lookup"><span data-stu-id="7b559-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="7b559-120">**Потребители в облака** – всеки Office 365 (O365) платен SKU или Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="7b559-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="7b559-121">**Облак и/или локални потребители** – Azure ad Premium P1 или P2, корпоративна мобилност + защита (EMS) или защитено продуктивно предприятие (спе)</span><span class="sxs-lookup"><span data-stu-id="7b559-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="7b559-122">За да научите повече за изискванията за лицензиране, вижте [лицензионни изисквания за услугата за самостоятелно нулиране на пароли на AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="7b559-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="7b559-123">За да нулирате паролата на потребител, намерете потребителя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7b559-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="7b559-124">След това щракнете върху бутона "нулиране на паролата" в острието на прегледа за този потребител.</span><span class="sxs-lookup"><span data-stu-id="7b559-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="7b559-125">**Бутонът за нулиране на паролата е сив**</span><span class="sxs-lookup"><span data-stu-id="7b559-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="7b559-126">Не сте упълномощени да нулирате паролите на **този** потребител.</span><span class="sxs-lookup"><span data-stu-id="7b559-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="7b559-127">*Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.*</span><span class="sxs-lookup"><span data-stu-id="7b559-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7b559-128">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="7b559-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="7b559-129">**Не виждам Блейд за нулиране на паролата**</span><span class="sxs-lookup"><span data-stu-id="7b559-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="7b559-130">Не сте упълномощени да нулирате паролите.</span><span class="sxs-lookup"><span data-stu-id="7b559-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="7b559-131">*Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.*</span><span class="sxs-lookup"><span data-stu-id="7b559-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7b559-132">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="7b559-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="7b559-133">**Не виждам острието на локалната интеграция при нулиране на паролата**</span><span class="sxs-lookup"><span data-stu-id="7b559-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="7b559-134">В хибридни среди се показва локалният нож за интегриране, което означава, че използвате Password нефиксирани за манипулиране на пароли на локални потребители.</span><span class="sxs-lookup"><span data-stu-id="7b559-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="7b559-135">Не виждате това острие, ако:</span><span class="sxs-lookup"><span data-stu-id="7b559-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="7b559-136">Не използвате Password нефиксирани</span><span class="sxs-lookup"><span data-stu-id="7b559-136">You are not using password writeback</span></span>
  - <span data-ttu-id="7b559-137">Има проблем с вашата инсталация/свързване на парола нефиксирани</span><span class="sxs-lookup"><span data-stu-id="7b559-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="7b559-138">Има проблем с вашата инсталация/свързване на Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7b559-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="7b559-139">За повече стъпки за отстраняване на проблеми с Password нефиксирани вижте [отстраняване на проблеми с паролата нефиксирани](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="7b559-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="7b559-140">**Не знам как да нулирам паролата на потребител**</span><span class="sxs-lookup"><span data-stu-id="7b559-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="7b559-141">Влезте в портала на Azure като подходящ администратор.</span><span class="sxs-lookup"><span data-stu-id="7b559-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="7b559-142">Отидете на острието **потребители и групи** , изберете **всички потребители**.</span><span class="sxs-lookup"><span data-stu-id="7b559-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="7b559-143">Изберете потребител от списъка.</span><span class="sxs-lookup"><span data-stu-id="7b559-143">Select a user from the list.</span></span>
4. <span data-ttu-id="7b559-144">За избрания потребител изберете **Обзор** и след това в командната лента изберете **нулиране на парола**.</span><span class="sxs-lookup"><span data-stu-id="7b559-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="7b559-145">Изберете бутона за **нулиране на паролата** , след което следвайте инструкциите на екрана.</span><span class="sxs-lookup"><span data-stu-id="7b559-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="7b559-146">Извършва се само нулирания чрез портала за поддръжка на нефиксирани на **Azure** .</span><span class="sxs-lookup"><span data-stu-id="7b559-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="7b559-147">**Нулирам паролата за локален потребител от портала за администриране на Office 365 или мобилното приложение на Office 365, но потребителят все още не може да влезе**</span><span class="sxs-lookup"><span data-stu-id="7b559-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="7b559-148">Парола нефиксирани не се поддържа в този портал.</span><span class="sxs-lookup"><span data-stu-id="7b559-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="7b559-149">Нулирайте отново паролата на потребителя в портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="7b559-149">Reset the user's password again in the Azure portal.</span></span>
