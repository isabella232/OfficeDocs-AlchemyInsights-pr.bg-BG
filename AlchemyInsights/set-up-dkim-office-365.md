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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645661"
---
# <a name="setup-dkim"></a><span data-ttu-id="6e6c9-102">Настройка на DKIM</span><span class="sxs-lookup"><span data-stu-id="6e6c9-102">Setup DKIM</span></span>

<span data-ttu-id="6e6c9-103">Пълните инструкции за конфигуриране на DKIM за персонализирани домейни в Microsoft 365 са [тук](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6e6c9-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="6e6c9-104">За **всеки** персонализиран домейн трябва да създадете **два** DKIM CNAME записа на DNS хостинг услуга на домейна си (обикновено, регистраторът на домейни).</span><span class="sxs-lookup"><span data-stu-id="6e6c9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="6e6c9-105">Например contoso.com и fourthcoffee.com изискват четири DKIM CNAME записа: два за contoso.com и два за fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="6e6c9-106">DKIM CNAME записи за **всеки** домейн използва следните формати:</span><span class="sxs-lookup"><span data-stu-id="6e6c9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="6e6c9-107">**Име на хоста:**`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6e6c9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6e6c9-108">**Точки за адрес или стойност:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6e6c9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6e6c9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6e6c9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="6e6c9-110">**Име на хоста:**`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6e6c9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6e6c9-111">**Точки за адрес или стойност:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6e6c9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6e6c9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6e6c9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="6e6c9-113">\<DomainGUID\> е текст ът `.mail.protection.outlook.com` отляво на потребителски MX запис за домейна по избор (например `contoso-com` домейн contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6e6c9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="6e6c9-114">\<InitialDomain\> е домейнът, който сте използвали, когато сте се регистрирали за Microsoft 365 (например contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="6e6c9-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="6e6c9-115">След като сте създали CNAME записи за вашите персонализирани домейни, изпълнете следните инструкции:</span><span class="sxs-lookup"><span data-stu-id="6e6c9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="6e6c9-116">A.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-116">a.</span></span> <span data-ttu-id="6e6c9-117">[влезете в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с вашия служебен или учебен акаунт.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="6e6c9-118">B.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-118">b.</span></span> <span data-ttu-id="6e6c9-119">Изберете иконата за стартиране на приложения в горния ляв ъгъл и изберете **Администратор**.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="6e6c9-120">C.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-120">c.</span></span> <span data-ttu-id="6e6c9-121">В долната лява навигация разгънете **Администратор** и изберете **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="6e6c9-122">D.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-122">d.</span></span> <span data-ttu-id="6e6c9-123">Отидете на **Защита** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="6e6c9-124">E.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-124">e.</span></span> <span data-ttu-id="6e6c9-125">Изберете домейна и след това изберете **Разрешаване** за Подписване на **съобщения за този домейн с DKIM подписи**.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="6e6c9-126">Повторете тази стъпка за всеки персонализиран домейн.</span><span class="sxs-lookup"><span data-stu-id="6e6c9-126">Repeat this step for each custom domain.</span></span>
