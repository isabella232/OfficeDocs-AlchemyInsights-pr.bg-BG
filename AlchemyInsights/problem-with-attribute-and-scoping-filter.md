---
title: Проблем с филтъра "атрибут и обхват"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480970"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="247dc-102">Проблем с филтъра "атрибут и обхват"</span><span class="sxs-lookup"><span data-stu-id="247dc-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="247dc-103">**Проблем със противоречиви UPN стойности**</span><span class="sxs-lookup"><span data-stu-id="247dc-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="247dc-104">Работният ден за осигуряване на работен ден на потребителя за реклама на ad потребители показва съобщение за грешка **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="247dc-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="247dc-105">Операцията е неуспешна, защото UPN стойност, предоставена за добавяне/модификация, не е уникална за цялата гора.</span><span class="sxs-lookup"><span data-stu-id="247dc-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="247dc-106">Подробни данни за грешка: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="247dc-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="247dc-107">Стойността на **userPrincipalName** , която се опитва да зададе вашият работен лист, когато се създава потребителският АКАУНТ за реклама, вече съществува в целевия домейн за реклама.</span><span class="sxs-lookup"><span data-stu-id="247dc-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="247dc-108">Това означава, че или (1) потребителят вече съществува и че ИД на съвпадението не е неуспешно за потребителя или (2) правилото за UPN поколение генерира конфликтна стойност.</span><span class="sxs-lookup"><span data-stu-id="247dc-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="247dc-109">По-долу са описани стъпките за предложения за разрешаване:</span><span class="sxs-lookup"><span data-stu-id="247dc-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="247dc-110">Ако потребителят вече съществува и проверката за съвпадащи ИД е неуспешна, за да се свърже акаунтът за работен ден към акаунт за Active Directory, тогава Проверете дали Атрибутът за съвпадащи ИД (обикновено **employeeID**) както в работен ден, така и в рекламата има точно съвпадение.</span><span class="sxs-lookup"><span data-stu-id="247dc-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="247dc-111">Ако не съвпадат, това е проблем с данни, който трябва да бъде коригиран.</span><span class="sxs-lookup"><span data-stu-id="247dc-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="247dc-112">Например, ако EmployeeID в работен ден е 001052, а в AD то е 1052, тогава Осигуряващият двигател няма да може да свърже двата акаунта и ще се опита да създаде потребител, който вече съществува.</span><span class="sxs-lookup"><span data-stu-id="247dc-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="247dc-113">В този случай решението е да се промени стойността на **EmployeeID** в ad, за да се включат водещите нули, за да бъдат 001052.</span><span class="sxs-lookup"><span data-stu-id="247dc-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="247dc-114">Ако изразът генериращ UPN не генерира уникална стойност, помислете за използване на функцията за дублиране на **SelectUniqueValue** , за да генерирате уникална стойност всеки път.</span><span class="sxs-lookup"><span data-stu-id="247dc-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="247dc-115">**Осигуряването на работен ден на AD потребители не задава стойност на атрибута "мениджър" за потребителския акаунт за реклама**</span><span class="sxs-lookup"><span data-stu-id="247dc-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="247dc-116">Заданието за осигуряване на работен ден за реклама на потребителя не задава стойността на атрибута **Manager** за потребителските акаунти за реклама.</span><span class="sxs-lookup"><span data-stu-id="247dc-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="247dc-117">Има два възможни сценария, когато се вижда това поведение:</span><span class="sxs-lookup"><span data-stu-id="247dc-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="247dc-118">Ръководителят в работен ден не може да бъде разрешен за съответен потребителски акаунт за реклама, тъй като диспечерът не е в обхват.</span><span class="sxs-lookup"><span data-stu-id="247dc-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="247dc-119">В сценария с **множество рекламни домейни** Диспечерът в работен ден не присъства в същия домейн като потребителя.</span><span class="sxs-lookup"><span data-stu-id="247dc-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="247dc-120">Изпробвайте тези стъпки, за да отстраните проблема:</span><span class="sxs-lookup"><span data-stu-id="247dc-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="247dc-121">Ако сте определили филтри за обхват, първо проверете дали Ръководителят е в обхвата си и че отговаря на клаузата за обхват.</span><span class="sxs-lookup"><span data-stu-id="247dc-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="247dc-122">Ако диспечерът не отговаря на филтъра за обхват, променете филтъра, така че ръководителят да е в обхвата на операцията за осигуряване.</span><span class="sxs-lookup"><span data-stu-id="247dc-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="247dc-123">Ако имате множество домейни за реклама, тогава Конекторът има известно ограничение за неспособност за разрешаване на препратките към диспечера за кръстосани домейни.</span><span class="sxs-lookup"><span data-stu-id="247dc-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="247dc-124">За повече информация за конфигурирането на работен ден за автоматизирано осигуряване вижте [урок: Конфигуриране на работен ден за автоматично осигуряване на потребителя](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="247dc-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













