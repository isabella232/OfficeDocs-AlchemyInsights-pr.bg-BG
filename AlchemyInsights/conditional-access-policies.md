---
title: Правила за условен достъп
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100394"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="1e3b5-102">Правила за условен достъп</span><span class="sxs-lookup"><span data-stu-id="1e3b5-102">Conditional Access policies</span></span>

<span data-ttu-id="1e3b5-103">Условен достъп е възможност за Azure AD, която ви позволява да прилагате контроли на достъпа до приложенията във вашата среда, като всички те се базират на конкретни условия и се управляват от централно местоположение.</span><span class="sxs-lookup"><span data-stu-id="1e3b5-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="1e3b5-104">Научете повече за[условен достъп в Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="1e3b5-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="1e3b5-105">**Бележка**: Ако вашият клиент е създаден след 21 октомври 2019 г. и неочаквано получите подкана за многофакторно удостоверяване (MFA), вероятно имате разрешени [настройки по подразбиране за защита,](http://aka.ms/securitydefaults) във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="1e3b5-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="1e3b5-106">**За да управлявате настройките по подразбиране за защита**</span><span class="sxs-lookup"><span data-stu-id="1e3b5-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="1e3b5-107">Влезте в [центъра за администриране](https://go.microsoft.com/fwlink/p/?linkid=834822) с идентификационните си данни на глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="1e3b5-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="1e3b5-108">Отидете на [свойства на Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="1e3b5-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="1e3b5-109">В долния край на страницата щракнете върху **Управление на настройките по подразбиране за защита**.</span><span class="sxs-lookup"><span data-stu-id="1e3b5-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="1e3b5-110">Щракнете върху **Да**, за да разрешите настройките по подразбиране за защита или върху **Не**, за да забраните настройките по подразбиране за защита.</span><span class="sxs-lookup"><span data-stu-id="1e3b5-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
