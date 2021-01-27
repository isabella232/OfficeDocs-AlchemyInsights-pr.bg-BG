---
title: Проблеми с достъпа под условие
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014722"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="dbac7-102">Проблеми с достъпа под условие</span><span class="sxs-lookup"><span data-stu-id="dbac7-102">Conditional access issues</span></span>

<span data-ttu-id="dbac7-103">**Отстраняване на проблеми с диагностичната идентификация**</span><span class="sxs-lookup"><span data-stu-id="dbac7-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="dbac7-104">Можете бързо да разберете какво се е случило или да диагностицирате проблеми, свързани с потребителското влизане, като използвате [диагностичната диагностика за влизане](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="dbac7-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="dbac7-105">Стартирайте диагностичната диагностика за влизане.</span><span class="sxs-lookup"><span data-stu-id="dbac7-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="dbac7-106">Намерете събитието, което искате да анализирате, като въведете подробностите, които имате за потребителя, приложението, часа на влизане, ИД на заявката или ИД на корелация.</span><span class="sxs-lookup"><span data-stu-id="dbac7-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="dbac7-107">Прегледайте диагностичните резултати, показващи подробностите за това какво се е случило и какви действия можете да предприемете, за да направите промени (ако са необходими промени).</span><span class="sxs-lookup"><span data-stu-id="dbac7-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="dbac7-108">**Стъпки за отстраняване на неизправности при влизане**</span><span class="sxs-lookup"><span data-stu-id="dbac7-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="dbac7-109">Придвижете се до страницата за влизане на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dbac7-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="dbac7-110">Филтрирайте регистрациите по потребител, времеви диапазон, приложение, състояние, клиентско приложение и т. н.</span><span class="sxs-lookup"><span data-stu-id="dbac7-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="dbac7-111">Изберете събитие за влизане и Прегледайте раздела условен достъп, за да видите кои правила са оценени.</span><span class="sxs-lookup"><span data-stu-id="dbac7-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="dbac7-112">Щракнете върху реда на правилата, за да видите подробните данни за правилата и да разберете защо то е приложено.</span><span class="sxs-lookup"><span data-stu-id="dbac7-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="dbac7-113">**Инструменти за отстраняване на неизправности при правила за условен достъп**</span><span class="sxs-lookup"><span data-stu-id="dbac7-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="dbac7-114">Режим само за отчети ви позволява да оценявате правила, без да засягате потребители.</span><span class="sxs-lookup"><span data-stu-id="dbac7-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="dbac7-115">Инструментът If ви позволява да симулирате събития при влизане и да виждате кои правила се прилагат.</span><span class="sxs-lookup"><span data-stu-id="dbac7-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="dbac7-116">Работна книга за прозрения и отчитане показва въздействието в реално време на всяка политика.</span><span class="sxs-lookup"><span data-stu-id="dbac7-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="dbac7-117">**Правила за защита на базова линия**</span><span class="sxs-lookup"><span data-stu-id="dbac7-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="dbac7-118">Правилата за защита на базисни стойности бяха прекратени.</span><span class="sxs-lookup"><span data-stu-id="dbac7-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="dbac7-119">Те вече не се налагат и скоро ще бъдат премахнати от портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="dbac7-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="dbac7-120">Препоръчваме ви да разрешавате [настройките по подразбиране за защита](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="dbac7-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="dbac7-121">За повече информация относно условния достъп вижте:</span><span class="sxs-lookup"><span data-stu-id="dbac7-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="dbac7-122">[Най-добри практики за условен достъп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия в условния достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Контроли в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Местоположения в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="dbac7-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
