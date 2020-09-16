---
title: Създаване на релация към организация за разрешаване на потребителите да работят съвместно с друга организация
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712722"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="8665b-102">Създаване на релация към организация за разрешаване на потребителите да работят съвместно с друга организация</span><span class="sxs-lookup"><span data-stu-id="8665b-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="8665b-103">От таблото на центъра за администриране на Microsoft 365 отидете на **администратор**на  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="8665b-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="8665b-104">Отидете на **organization**  >  "**споделяне**на организация".</span><span class="sxs-lookup"><span data-stu-id="8665b-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="8665b-105">Под **споделяне на организация**щракнете върху **Създай** .</span><span class="sxs-lookup"><span data-stu-id="8665b-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="8665b-106">В **нова организация релация**, в полето **име на релация** въведете истинско име за релацията между организацията.</span><span class="sxs-lookup"><span data-stu-id="8665b-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="8665b-107">В полето **домейни за споделяне с** Въведете домейна за външни Office 365 или локална организация на Exchange, която искате да споделите с календарите си.</span><span class="sxs-lookup"><span data-stu-id="8665b-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="8665b-108">Ако трябва да въведете повече от един домейн, разделете имена на домейни със запетая.</span><span class="sxs-lookup"><span data-stu-id="8665b-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="8665b-109">Например contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="8665b-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="8665b-110">Изберете квадратчето за отметка **Разреши споделяне на информация за заетост от календара** , за да включите споделянето на календари с домейни, които сте записали.</span><span class="sxs-lookup"><span data-stu-id="8665b-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="8665b-111">Задаване на ниво на споделяне на информация за заетост от календара и Задайте кои потребители да могат да споделят информация за заетост от календара.</span><span class="sxs-lookup"><span data-stu-id="8665b-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="8665b-112">За да зададете ниво на достъп за заетост, изберете едно от следните неща:</span><span class="sxs-lookup"><span data-stu-id="8665b-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="8665b-113">**Информация за заетост от календара само с час**</span><span class="sxs-lookup"><span data-stu-id="8665b-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="8665b-114">**Календар свободен/зает с час, тема и местоположение**</span><span class="sxs-lookup"><span data-stu-id="8665b-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="8665b-115">За да зададете кои потребители да споделят информация за заетост от календара, изберете една от следните опции:</span><span class="sxs-lookup"><span data-stu-id="8665b-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="8665b-116">**Всеки във вашата организация**</span><span class="sxs-lookup"><span data-stu-id="8665b-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="8665b-117">**Посочена група за защита**</span><span class="sxs-lookup"><span data-stu-id="8665b-117">**A specified security group**</span></span>  

<span data-ttu-id="8665b-118">Щракнете върху **Преглед** , за да изберете групата защита от списък, след което щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="8665b-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="8665b-119">Щракнете върху **Запиши** , за да създадете релацията между организацията.</span><span class="sxs-lookup"><span data-stu-id="8665b-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="8665b-120">**Забележка:** Конфигурациите между клиенти не поддържат лични контакти за справки за заетост.</span><span class="sxs-lookup"><span data-stu-id="8665b-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="8665b-121">Контактите трябва да бъдат включени в глобалния адресен списък за работа със заетостта.</span><span class="sxs-lookup"><span data-stu-id="8665b-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="8665b-122">**За да разберете подробно тази тема, моля, прочетете:**</span><span class="sxs-lookup"><span data-stu-id="8665b-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="8665b-123">Създаване на организационна релация в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8665b-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="8665b-124">Промяна на релация на организация в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8665b-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="8665b-125">Премахване на релация на организация в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8665b-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
