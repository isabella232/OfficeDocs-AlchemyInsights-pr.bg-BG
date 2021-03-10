---
title: Нулиране на паролата за проблема
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692889"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="9efac-102">Проблеми при нулиране на паролата</span><span class="sxs-lookup"><span data-stu-id="9efac-102">Problems resetting password</span></span>

<span data-ttu-id="9efac-103">Следва някои от проблемите, които може да срещнете при нулиране на паролата и възможните решения:</span><span class="sxs-lookup"><span data-stu-id="9efac-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="9efac-104">**Имам проблем с нулирането на паролата, което не е включено в другите категории**</span><span class="sxs-lookup"><span data-stu-id="9efac-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="9efac-105">Уверете се, че сте упълномощени за нулиране на пароли.</span><span class="sxs-lookup"><span data-stu-id="9efac-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="9efac-106">Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.</span><span class="sxs-lookup"><span data-stu-id="9efac-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="9efac-107">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="9efac-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="9efac-108">Уверете се, че разбирате изискванията за лицензиране:</span><span class="sxs-lookup"><span data-stu-id="9efac-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="9efac-109">Трябва да имате поне един лиценз, присвоен във вашата организация</span><span class="sxs-lookup"><span data-stu-id="9efac-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="9efac-110">Потребители в облака – всеки Office 365 (O365) платен SKU или Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="9efac-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="9efac-111">Облак и/или локални потребители – Azure AD Premium P1 или P2, корпоративна мобилност + защита (EMS) или защитено продуктивно предприятие (СПЕ)</span><span class="sxs-lookup"><span data-stu-id="9efac-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="9efac-112">За да прочетете повече за изискванията за лицензиране, вижте статията [изисквания за лицензиране на услугата за самостоятелно нулиране на пароли на AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9efac-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9efac-113">**Имам проблеми с изпробването на правилата за нулиране на паролата, които задам**</span><span class="sxs-lookup"><span data-stu-id="9efac-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="9efac-114">Наскоро приложените правила могат да изминат няколко минути, за да се репликират във всички центрове за данни и крайните точки.</span><span class="sxs-lookup"><span data-stu-id="9efac-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="9efac-115">Физическото разстояние от центъра за данни ще засегне и колко бързо се прилагат промените.</span><span class="sxs-lookup"><span data-stu-id="9efac-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="9efac-116">Проверете при крайния потребител, а не като администратор и пилот с малък набор от потребители.</span><span class="sxs-lookup"><span data-stu-id="9efac-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="9efac-117">Правилата, конфигурирани в портала на Azure, се отнасят само за крайни потребители, но не и за администратори.</span><span class="sxs-lookup"><span data-stu-id="9efac-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="9efac-118">Microsoft налага строги правила за нулиране на пароли с две порти за всяка роля на администратор на Azure (пример: глобален администратор, администратор на Helpdesk, администратор на пароли и др.)</span><span class="sxs-lookup"><span data-stu-id="9efac-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="9efac-119">Научете повече за [правилата за администраторите](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="9efac-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="9efac-120">**Искам да разположи нулирането на паролата, но не искам да правя така, че моите потребители да регистрират допълнителна информация за защита**</span><span class="sxs-lookup"><span data-stu-id="9efac-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="9efac-121">Предварително попълнени данни за вашите потребители, така че да не е необходимо!</span><span class="sxs-lookup"><span data-stu-id="9efac-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="9efac-122">-Като администратор можете да настроите свойствата на телефона и имейла за вашите потребители, преди да се стартира нулирането на паролата за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="9efac-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="9efac-123">Можете да направите това с помощта на API, PowerShell или Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9efac-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="9efac-124">Повече информация тук:</span><span class="sxs-lookup"><span data-stu-id="9efac-124">More information here:</span></span>
- [<span data-ttu-id="9efac-125">Разполагане на нулиране на паролата, без да се изисква регистрация на потребителите</span><span class="sxs-lookup"><span data-stu-id="9efac-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="9efac-126">Какви данни се използват чрез нулиране на паролата</span><span class="sxs-lookup"><span data-stu-id="9efac-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="9efac-127">**Бутонът за нулиране на паролата е сив**</span><span class="sxs-lookup"><span data-stu-id="9efac-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="9efac-128">Не сте упълномощени да нулирате паролите на този потребител.</span><span class="sxs-lookup"><span data-stu-id="9efac-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="9efac-129">Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.</span><span class="sxs-lookup"><span data-stu-id="9efac-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="9efac-130">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="9efac-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="9efac-131">**Не виждам Блейд за нулиране на паролата**</span><span class="sxs-lookup"><span data-stu-id="9efac-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="9efac-132">Не сте упълномощени да нулирате паролите.</span><span class="sxs-lookup"><span data-stu-id="9efac-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="9efac-133">Само глобални, Password и потребителски администратори могат да нулират потребителските пароли.</span><span class="sxs-lookup"><span data-stu-id="9efac-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="9efac-134">Глобалните администратори могат да нулират и паролите на други привилегировани администратори.</span><span class="sxs-lookup"><span data-stu-id="9efac-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="9efac-135">**Не виждам острието на локалната интеграция при нулиране на паролата**</span><span class="sxs-lookup"><span data-stu-id="9efac-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="9efac-136">В хибридни среди се показва локалният нож за интегриране, което означава, че използвате Password нефиксирани за манипулиране на пароли на локални потребители.</span><span class="sxs-lookup"><span data-stu-id="9efac-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="9efac-137">Не виждате това острие, ако:</span><span class="sxs-lookup"><span data-stu-id="9efac-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="9efac-138">Не използвате Password нефиксирани</span><span class="sxs-lookup"><span data-stu-id="9efac-138">You are not using password writeback</span></span>
    - <span data-ttu-id="9efac-139">Има проблем с вашата инсталация/свързване на парола нефиксирани</span><span class="sxs-lookup"><span data-stu-id="9efac-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="9efac-140">Има проблем с вашата инсталация/свързване на Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9efac-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="9efac-141">За повече стъпки за отстраняване на неизправности при проблеми с Password нефиксирани, вижте раздела [отстраняване на неизправности при парола нефиксирани](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="9efac-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="9efac-142">**Не знам как да нулирам паролата на потребител**</span><span class="sxs-lookup"><span data-stu-id="9efac-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="9efac-143">Влезте в портала на Azure като подходящ администратор.</span><span class="sxs-lookup"><span data-stu-id="9efac-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="9efac-144">Отидете на острието потребители и групи, изберете **всички потребители**.</span><span class="sxs-lookup"><span data-stu-id="9efac-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="9efac-145">Изберете потребител от списъка.</span><span class="sxs-lookup"><span data-stu-id="9efac-145">Select a user from the list.</span></span>
1. <span data-ttu-id="9efac-146">За избрания потребител изберете **Обзор** и след това в командната лента щракнете върху **нулиране на парола**.</span><span class="sxs-lookup"><span data-stu-id="9efac-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="9efac-147">Следвайте инструкциите на екрана.</span><span class="sxs-lookup"><span data-stu-id="9efac-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="9efac-148">Извършва се само нулирания чрез портала за поддръжка на нефиксирани на Azure.</span><span class="sxs-lookup"><span data-stu-id="9efac-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="9efac-149">**Нулирам паролата за локален потребител от портала за администриране на Office 365 или мобилното приложение на Office 365, но потребителят все още не може да влезе**</span><span class="sxs-lookup"><span data-stu-id="9efac-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="9efac-150">Парола нефиксирани не се поддържа в този портал.</span><span class="sxs-lookup"><span data-stu-id="9efac-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="9efac-151">Нулиране на паролата на потребител отново в портала на Azure – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="9efac-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

