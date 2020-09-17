---
title: Настройки на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808696"
---
# <a name="setup-dkim"></a><span data-ttu-id="cf78e-102">Настройки на DKIM</span><span class="sxs-lookup"><span data-stu-id="cf78e-102">Setup DKIM</span></span>

<span data-ttu-id="cf78e-103">Пълните инструкции за конфигуриране на DKIM за домейни по избор в Microsoft 365 са [тук](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="cf78e-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="cf78e-104">За **всеки** домейн по избор трябва да създадете **два** DKIM CNAME ЗАПИСА в услугата за DNS хостинг на вашия домейн (обикновено регистраторът на домейни).</span><span class="sxs-lookup"><span data-stu-id="cf78e-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="cf78e-105">Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: две за contoso.com и две за fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="cf78e-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="cf78e-106">DKIM CNAME Records за **всеки** домейн по избор използва следните формати:</span><span class="sxs-lookup"><span data-stu-id="cf78e-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="cf78e-107">**Име на хост**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf78e-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf78e-108">**Сочи към адрес или стойност**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf78e-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf78e-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf78e-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="cf78e-110">**Име на хост**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf78e-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf78e-111">**Сочи към адрес или стойност**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf78e-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf78e-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf78e-112">**TTL**: 3600</span></span>

   <span data-ttu-id="cf78e-113">\<DomainGUID\> е текстът отляво на `.mail.protection.outlook.com` в персонализирания MX запис за домейна по избор (например `contoso-com` за домейна contoso.com).</span><span class="sxs-lookup"><span data-stu-id="cf78e-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="cf78e-114">\<InitialDomain\> е домейнът, който сте използвали, когато сте се записали за Microsoft 365 (например contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="cf78e-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="cf78e-115">След като сте създали CNAME записите за вашите домейни по избор, изпълнете следните инструкции:</span><span class="sxs-lookup"><span data-stu-id="cf78e-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="cf78e-116">на.</span><span class="sxs-lookup"><span data-stu-id="cf78e-116">a.</span></span> <span data-ttu-id="cf78e-117">[Влезте в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) със своя служебен или учебен акаунт.</span><span class="sxs-lookup"><span data-stu-id="cf78e-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="cf78e-118">b.</span><span class="sxs-lookup"><span data-stu-id="cf78e-118">b.</span></span> <span data-ttu-id="cf78e-119">Изберете иконата за стартиране на приложения в горния ляв ъгъл и изберете **администратор**.</span><span class="sxs-lookup"><span data-stu-id="cf78e-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="cf78e-120">c.</span><span class="sxs-lookup"><span data-stu-id="cf78e-120">c.</span></span> <span data-ttu-id="cf78e-121">В навигацията в долния ляв ъгъл разгънете **администратор** и изберете **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="cf78e-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="cf78e-122">d.</span><span class="sxs-lookup"><span data-stu-id="cf78e-122">d.</span></span> <span data-ttu-id="cf78e-123">Отидете на **Protection**  >  **DKIM**за защита.</span><span class="sxs-lookup"><span data-stu-id="cf78e-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="cf78e-124">e.</span><span class="sxs-lookup"><span data-stu-id="cf78e-124">e.</span></span> <span data-ttu-id="cf78e-125">Изберете домейна и след това изберете **Разрешаване** на **подписване на съобщения за този домейн с подписи на DKIM**.</span><span class="sxs-lookup"><span data-stu-id="cf78e-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="cf78e-126">Повторете тази стъпка за всеки домейн по избор.</span><span class="sxs-lookup"><span data-stu-id="cf78e-126">Repeat this step for each custom domain.</span></span>
