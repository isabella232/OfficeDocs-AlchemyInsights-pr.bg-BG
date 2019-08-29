---
title: Настройка DKIM в Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666253"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="397c4-102">Настройка DKIM в Office 365</span><span class="sxs-lookup"><span data-stu-id="397c4-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="397c4-103">Пълни инструкции за конфигуриране DKIM за потребителски домейни в Office 365 са [тук](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="397c4-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="397c4-104">За **всеки** потребителски домейн трябва да създадете **две** DKIM CNAME записите в хостинг услугата за вашия домейн DNS (обикновено, регистраторът на домейни).</span><span class="sxs-lookup"><span data-stu-id="397c4-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="397c4-105">Например contoso.com и fourthcoffee.com изисква четири DKIM CNAME записи: две за contoso.com и два за fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="397c4-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="397c4-106">DKIM CNAME записи за **всеки** потребителски домейн използва следните формати:</span><span class="sxs-lookup"><span data-stu-id="397c4-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="397c4-107">**Име на хост**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="397c4-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="397c4-108">**Точки за адрес или стойност**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="397c4-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="397c4-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="397c4-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="397c4-110">**Име на хост**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="397c4-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="397c4-111">**Точки за адрес или стойност**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="397c4-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="397c4-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="397c4-112">**TTL**: 3600</span></span>

   <span data-ttu-id="397c4-113">\<DomainGUID\> е текст от ляво на `.mail.protection.outlook.com` в потребителски MX записа за собствен домейн (например, `contoso-com` за домейна contoso.com).</span><span class="sxs-lookup"><span data-stu-id="397c4-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="397c4-114">\<InitialDomain\> е домейн сте използвали, когато сте се регистрирали за Office 365 (например, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="397c4-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="397c4-115">След като сте създали CNAME записи за вашите потребителски домейни, изпълнете следните инструкции:</span><span class="sxs-lookup"><span data-stu-id="397c4-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="397c4-116">a.</span><span class="sxs-lookup"><span data-stu-id="397c4-116">a.</span></span> <span data-ttu-id="397c4-117">[Влезте в Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с профила си работа или училище.</span><span class="sxs-lookup"><span data-stu-id="397c4-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="397c4-118">б.</span><span class="sxs-lookup"><span data-stu-id="397c4-118">b.</span></span> <span data-ttu-id="397c4-119">Изберете иконата на стартера на ап в горния ляв и **администратор**.</span><span class="sxs-lookup"><span data-stu-id="397c4-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="397c4-120">c.</span><span class="sxs-lookup"><span data-stu-id="397c4-120">c.</span></span> <span data-ttu-id="397c4-121">В долния ляв навигация разгънете **администратор** и изберете **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="397c4-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="397c4-122">d.</span><span class="sxs-lookup"><span data-stu-id="397c4-122">d.</span></span> <span data-ttu-id="397c4-123">Отидете на **защита** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="397c4-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="397c4-124">д.</span><span class="sxs-lookup"><span data-stu-id="397c4-124">e.</span></span> <span data-ttu-id="397c4-125">Изберете домейн и след това изберете **Разреши** за **знак за съобщенията за този домейн с DKIM подписи**.</span><span class="sxs-lookup"><span data-stu-id="397c4-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="397c4-126">Повторете тази стъпка за всеки домейн.</span><span class="sxs-lookup"><span data-stu-id="397c4-126">Repeat this step for each custom domain.</span></span>
