---
title: Приложение за удостоверяване
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404249"
---
# <a name="authentication-app"></a><span data-ttu-id="ee59c-102">Приложение за удостоверяване</span><span class="sxs-lookup"><span data-stu-id="ee59c-102">Authentication app</span></span>

<span data-ttu-id="ee59c-103">Ако сте глобален администратор, можете бързо да разберете какво се е случило или да диагностицирате проблеми, свързани с влизането на потребителя, с помощта [на диагностиката за влизане.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="ee59c-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="ee59c-104">Стартирайте диагностиката, като щракнете върху бутона["Стартиране на](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)диагностиката".</span><span class="sxs-lookup"><span data-stu-id="ee59c-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="ee59c-105">Намерете събитието, за да анализирате, като въведете подробните данни за потребителя, приложението, часа на влизане, ИД на заявка или ИД на корелация.</span><span class="sxs-lookup"><span data-stu-id="ee59c-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="ee59c-106">Прегледайте диагностичните резултати, показващи подробностите за случилото се и какви действия можете да предприемете, за да направите промени, ако са необходими някакви промени.</span><span class="sxs-lookup"><span data-stu-id="ee59c-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="ee59c-107">**Проверете сценария, който е приложим:**</span><span class="sxs-lookup"><span data-stu-id="ee59c-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="ee59c-108">Ако потребителят не получава push известие в приложението Microsoft Authenticator, проверете дали не се показват под блокираните потребители на MFA, както е описано [в Блокиране и разблокиране на потребители.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="ee59c-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="ee59c-109">Ако потребителят не е блокиран за MFA, но не получи push известие, той може да отвори приложението Microsoft Authenticator, което ще изтегли чакащите искания за одобрение.</span><span class="sxs-lookup"><span data-stu-id="ee59c-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="ee59c-110">Като алтернативен метод за влизане потребителят може също да щракне върху Влизане по друг начин и да избере да използва код за потвърждение от мобилното ми приложение.</span><span class="sxs-lookup"><span data-stu-id="ee59c-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="ee59c-111">Приложението Microsoft Authenticator е единственият наличен метод за много потребители.</span><span class="sxs-lookup"><span data-stu-id="ee59c-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="ee59c-112">[Научете повече за настройките по подразбиране за защита,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)проверете [ЧЗВ за приложението Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) за често задавани въпроси и как да ги разрешите.</span><span class="sxs-lookup"><span data-stu-id="ee59c-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="ee59c-113">**Препоръчителни видеоклипове**</span><span class="sxs-lookup"><span data-stu-id="ee59c-113">**Recommended Videos**</span></span>

<span data-ttu-id="ee59c-114">[Как да настроите приложението Authenticator на нов телефон (2 минути).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="ee59c-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
