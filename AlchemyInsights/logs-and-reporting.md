---
title: Регистрационни файлове и отчети
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035840"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="b9d6c-102">Регистрационни файлове и отчети</span><span class="sxs-lookup"><span data-stu-id="b9d6c-102">Logs and Reporting</span></span>

<span data-ttu-id="b9d6c-103">[ЧЗВ за съобщаването на Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) често задавани въпроси за отчетите за Azure Active Directory (Azure ad).</span><span class="sxs-lookup"><span data-stu-id="b9d6c-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="b9d6c-104">За повече информация вижте [отчитане на Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="b9d6c-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="b9d6c-105">**Отстраняване на проблеми с проверката**</span><span class="sxs-lookup"><span data-stu-id="b9d6c-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="b9d6c-106">Ако имате проблеми с преглеждането на някои дейности по одит и липсващата дейност е в този [списък](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), моля, подайте билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="b9d6c-107">Ако имате проблеми с преглеждането на регистрационни файлове за проверка във вашия клиент, моля, подайте билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="b9d6c-108">Ако вашите дейности по одита не се показват веднага в портала на Azure, прегледайте нашата [информация за латентност](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) и изнесете билет за поддръжка, ако закъснението надвишава документираната латентност.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="b9d6c-109">Архивиране на регистрационни файлове за дейности на Azure AD</span><span class="sxs-lookup"><span data-stu-id="b9d6c-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="b9d6c-110">Ако не виждате всички одити за диапазона от дати, който сте избрали, можете да изтеглите до 250K редове (сортирани по най-новата) на влизане в портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="b9d6c-111">За повече информация вижте [изтегляне на дейности за проверка](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="b9d6c-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="b9d6c-112">**Отстраняване на проблеми при влизане**</span><span class="sxs-lookup"><span data-stu-id="b9d6c-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="b9d6c-113">Можете да виждате последните 30 дни от данните, ако имате лиценз за Azure AD Premium (P1 или P2) за своя клиент.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="b9d6c-114">Регистрациите са налични само за клиентите на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="b9d6c-115">Той не е наличен за безплатните или основните лицензирани наематели.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="b9d6c-116">Ако вашият клиент има лиценз за Premium P1 и не можете да видите регистрациите, прегледайте нашата [информация за латентност](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) и подадете билет за поддръжка, ако закъснението надвишава документираното закъснение.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="b9d6c-117">Ако не виждате всички регистрации за диапазона от дати, който сте избрали, имайте предвид, че можете да изтеглите до 250K редове (сортирани по най-новата версия) на влизане в портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="b9d6c-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="b9d6c-118">За повече информация вижте [изтегляне на дейности за влизане](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="b9d6c-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="b9d6c-119">**Отстраняване на неизправности при отчетите за защита (потребители с флаг на риск, рискови влизане)**</span><span class="sxs-lookup"><span data-stu-id="b9d6c-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="b9d6c-120">Потребители с флаг за отчет за защита от рискове</span><span class="sxs-lookup"><span data-stu-id="b9d6c-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="b9d6c-121">Отчет за рискови регистрации в портала на Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b9d6c-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="b9d6c-122">Рискови събития за Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b9d6c-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
