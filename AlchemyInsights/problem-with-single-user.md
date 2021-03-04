---
title: Проблем с един потребител
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429347"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="53db3-102">Проблем с един потребител</span><span class="sxs-lookup"><span data-stu-id="53db3-102">Problem with single user</span></span>

- <span data-ttu-id="53db3-103">Потребителят може да не е осигурен, защото услугата все още не е успяла да оцени потребителя.</span><span class="sxs-lookup"><span data-stu-id="53db3-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="53db3-104">Прегледайте ръководството за продължителността на осигуряването, както и лентата за напредък на страницата за конфигуриране на обезпечаването.</span><span class="sxs-lookup"><span data-stu-id="53db3-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="53db3-105">Ако стационарното състояние, зададено в секцията допълнителни данни, е преди датата, на която потребителят е бил създаден/актуализиран/изтрит, това означава, че все още не сме оценили потребителя.</span><span class="sxs-lookup"><span data-stu-id="53db3-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="53db3-106">В този случай най-доброто нещо, което трябва да направите, е да изчакате услугата за осигуряване да завърши.</span><span class="sxs-lookup"><span data-stu-id="53db3-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="53db3-107">Имайте предвид, че нашата услуга е наясно само за промените в даден потребител в системата източник (ВП на облака).</span><span class="sxs-lookup"><span data-stu-id="53db3-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="53db3-108">Трябва да има валидна промяна в системата източник за Azure AD за откриване на промяната и преливането й в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53db3-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="53db3-109">Услугата за осигуряване е изчислила потребителя и е решила, че не трябва да бъде осигурена:</span><span class="sxs-lookup"><span data-stu-id="53db3-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="53db3-110">Ако сте задали филтър за обхват на обхвата на атрибута, уверете се, че потребителят отговаря на критериите, които сте задали.</span><span class="sxs-lookup"><span data-stu-id="53db3-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="53db3-111">Ако потребителите вече съществуват в целевата система и състоянието на потребителя в изходния и таргетния мач, няма да предприемем никакви последващи действия.</span><span class="sxs-lookup"><span data-stu-id="53db3-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="53db3-112">Услугата за осигуряване се опитва да осигури на потребителя и е неуспешна.</span><span class="sxs-lookup"><span data-stu-id="53db3-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="53db3-113">За тези сценарии Прегледайте раздела за отстраняване на неизправности и препоръки на регистрите за осигуряване:</span><span class="sxs-lookup"><span data-stu-id="53db3-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="53db3-114">Необходим атрибут на потребителя може да липсва в локалната Active Directory или Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53db3-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="53db3-115">Например правилата за създаване на userPrincipalName или sAMAccountName не генерират правилната стойност.</span><span class="sxs-lookup"><span data-stu-id="53db3-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="53db3-116">Атрибутът Match (обикновено employeeId) не се разрешава на уникален потребител в локален Active Directory или Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53db3-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="53db3-117">Например има два потребители с една и съща employeeId в AD и услугата връща код на грешка, за да се покаже дублирани записи за цел за един и същ запис източник.</span><span class="sxs-lookup"><span data-stu-id="53db3-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="53db3-118">За да прегледате регистрите за един потребител и групи, вижте [Преглед на осигуряването на регистрационни файлове за проблем с конкретен потребител](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="53db3-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
