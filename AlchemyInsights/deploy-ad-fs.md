---
title: Разполагане на AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177374"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="f7fbd-102">Разполагане на AD FS</span><span class="sxs-lookup"><span data-stu-id="f7fbd-102">Deploy AD FS</span></span>

<span data-ttu-id="f7fbd-103">Разполагането на услугите на Active Directory (AD FS) използва вашата локална инфраструктура за удостоверяване на потребители за услугите на Office 365.</span><span class="sxs-lookup"><span data-stu-id="f7fbd-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="f7fbd-104">С външно влизане можете да позволите на потребителите да влизат в услуги и софтуер на Office 365 като приложения на Service (SAAS), които са интегрирани с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f7fbd-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f7fbd-105">Външното влизане удостоверява потребители срещу вашия локален указател Active Directory чрез AD FS.</span><span class="sxs-lookup"><span data-stu-id="f7fbd-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="f7fbd-106">Освен това, докато сте в корпоративната мрежа, потребителите няма да бъдат задължени да въвеждат отново паролите си.</span><span class="sxs-lookup"><span data-stu-id="f7fbd-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="f7fbd-107">[Съветникът за разполагане на AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) ви предоставя инструкции "стъпка по стъпка" за разполагане на локален ИНФРАСТРУКТУРЕН AD FS, който удостоверява потребители за Microsoft 365 и Office 365 Services.</span><span class="sxs-lookup"><span data-stu-id="f7fbd-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="f7fbd-108">С това ръководство вашата организация може да преглежда компоненти и изисквания на AD FS, да придобива и инсталира SSL сертификати, които са необходими за разполагане, и да инсталира задължително прокси сървър на уеб приложението.</span><span class="sxs-lookup"><span data-stu-id="f7fbd-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
