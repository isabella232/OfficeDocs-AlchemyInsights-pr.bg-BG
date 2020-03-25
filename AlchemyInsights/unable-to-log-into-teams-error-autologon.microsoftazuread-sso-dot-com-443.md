---
title: Не е възможно влизане в Teams поради грешка autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931798"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="43eaf-102">Не е възможно влизане в Teams поради грешка autologon.microsoftazuread-sso точка com:443</span><span class="sxs-lookup"><span data-stu-id="43eaf-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="43eaf-103">Ако Seamless SSO е разрешено като удостоверяване на O365, може да е необходимо URL адресът autologon.microsoftazuread-sso.com да се добави към "Интранет сайтове".</span><span class="sxs-lookup"><span data-stu-id="43eaf-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="43eaf-104">Ако той вече е добавен към "Надеждни сайтове", при използване на Seamless SSO той трябва да бъде премахнат от "Надеждни сайтове".</span><span class="sxs-lookup"><span data-stu-id="43eaf-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="43eaf-105">Прегледайте [контролен списък за отстраняване на неизправности със Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="43eaf-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="43eaf-106">Изпълнете следните стъпки, за да добавите URL адрес към списъка "Интранет сайтове":</span><span class="sxs-lookup"><span data-stu-id="43eaf-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="43eaf-107">Отворете Internet Explorer, като щракнете върху бутона **Старт**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="43eaf-108">В полето за търсене въведете Internet Explorer и след това в списъка с резултати щракнете върху **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="43eaf-109">Щракнете върху **Инструменти** и след това – върху **Опции за интернет**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="43eaf-110">Щракнете върху раздела **Защита**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="43eaf-111">Сега щракнете върху **Локални интранет сайтове**, а след това щракнете върху бутона **Сайтове** и след това върху бутона **Разширени**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="43eaf-112">Въведете URL адреса на уеб сайта и щракнете върху **Добави**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="43eaf-113">Когато приключите, щракнете върху **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="43eaf-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="43eaf-114">За повече информация вж. [Документация за разполагане на Seamless SSO за O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (включва базиран на правила процес за добавяне на URL адрес към интранет сайтове в стъпка 3).</span><span class="sxs-lookup"><span data-stu-id="43eaf-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
