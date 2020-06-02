---
title: Настройка на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509373"
---
# <a name="setup-dkim"></a><span data-ttu-id="1081b-102">Настройка на DKIM</span><span class="sxs-lookup"><span data-stu-id="1081b-102">Setup DKIM</span></span>

<span data-ttu-id="1081b-103">Пълните инструкции за конфигуриране на DKIM за потребителски домейни в Microsoft 365 са [тук.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="1081b-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="1081b-104">За **всеки** потребителски домейн трябва да създадете **два** DKIM CNAME записа в DNS хостинг услугата на домейна ви (обикновено регистратор на домейни).</span><span class="sxs-lookup"><span data-stu-id="1081b-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="1081b-105">Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: два за contoso.com и два за fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="1081b-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="1081b-106">DKIM CNAME записи за **всеки** домейн използва следните формати:</span><span class="sxs-lookup"><span data-stu-id="1081b-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="1081b-107">**Име на хост**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="1081b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="1081b-108">**Точки за адрес или стойност:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="1081b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="1081b-109">**1000**000 евро</span><span class="sxs-lookup"><span data-stu-id="1081b-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="1081b-110">**Име на хост**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="1081b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="1081b-111">**Точки за адрес или стойност:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="1081b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="1081b-112">**1000**000 евро</span><span class="sxs-lookup"><span data-stu-id="1081b-112">**TTL**: 3600</span></span>

   <span data-ttu-id="1081b-113">\<DomainGUID\>е текстът отляво на `.mail.protection.outlook.com` персонализирания MX запис за домейна по избор (например `contoso-com` за домейна contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1081b-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="1081b-114">\<InitialDomain\>е домейнът, който сте използвали при регистрация за Microsoft 365 (например contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="1081b-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="1081b-115">След като създадете записите CNAME за вашите потребителски домейни, изпълнете следните инструкции:</span><span class="sxs-lookup"><span data-stu-id="1081b-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="1081b-116">A.</span><span class="sxs-lookup"><span data-stu-id="1081b-116">a.</span></span> <span data-ttu-id="1081b-117">[влезте в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с вашия служебен или учебен акаунт.</span><span class="sxs-lookup"><span data-stu-id="1081b-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="1081b-118">B.</span><span class="sxs-lookup"><span data-stu-id="1081b-118">b.</span></span> <span data-ttu-id="1081b-119">Изберете иконата на стартера на приложението в горния ляв ъгъл и изберете **Администриране**.</span><span class="sxs-lookup"><span data-stu-id="1081b-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="1081b-120">C.</span><span class="sxs-lookup"><span data-stu-id="1081b-120">c.</span></span> <span data-ttu-id="1081b-121">В навигацията в долния ляв ъгъл разгънете **Администратор** и изберете **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1081b-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="1081b-122">D.</span><span class="sxs-lookup"><span data-stu-id="1081b-122">d.</span></span> <span data-ttu-id="1081b-123">Отидете на **Защита**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="1081b-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="1081b-124">E.</span><span class="sxs-lookup"><span data-stu-id="1081b-124">e.</span></span> <span data-ttu-id="1081b-125">Изберете домейна и след това изберете **Разрешаване** за **подписване на съобщения за този домейн с DKIM подписи**.</span><span class="sxs-lookup"><span data-stu-id="1081b-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="1081b-126">Повторете тази стъпка за всеки домейн по избор.</span><span class="sxs-lookup"><span data-stu-id="1081b-126">Repeat this step for each custom domain.</span></span>
