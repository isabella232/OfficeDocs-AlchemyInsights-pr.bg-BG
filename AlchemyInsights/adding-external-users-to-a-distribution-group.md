---
title: Добавяне на външни потребители към група за разпространение
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737862"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d9b27-102">Добавяне на външни потребители към група за разпространение</span><span class="sxs-lookup"><span data-stu-id="d9b27-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d9b27-103">Добавяне на външен контакт към група за разпространение (ГД) е двуетаг процес:</span><span class="sxs-lookup"><span data-stu-id="d9b27-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d9b27-104">Създаване на имейл контакт за външен потребител:</span><span class="sxs-lookup"><span data-stu-id="d9b27-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d9b27-105">В центъра за администриране отидете на страницата с \*\*\*\* > [Контакти](https://admin.microsoft.com/adminportal/home#/Contact) на потребителите.</span><span class="sxs-lookup"><span data-stu-id="d9b27-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d9b27-106">Изберете **Добавяне на контакт**.</span><span class="sxs-lookup"><span data-stu-id="d9b27-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d9b27-107">Въведете информацията за вашия контакт и изберете **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="d9b27-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d9b27-108">Добавете имейл контакта към вашата ГД:</span><span class="sxs-lookup"><span data-stu-id="d9b27-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d9b27-109">В центъра за администриране отидете > на страницата групи \*\*\*\*[групи](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="d9b27-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d9b27-110">Намерете ГД, към която искате да добавите външен потребител, и я изберете, за да отворите диалога за редактиране.</span><span class="sxs-lookup"><span data-stu-id="d9b27-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d9b27-111">В раздела **членове** изберете Преглед на **всички и управление на членове**.</span><span class="sxs-lookup"><span data-stu-id="d9b27-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d9b27-112">Изберете **Добавяне на членове**.</span><span class="sxs-lookup"><span data-stu-id="d9b27-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d9b27-113">Изберете имейл контакта, който сте създали на предишната стъпка, след което изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="d9b27-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d9b27-114">Ако след следването на тези стъпки външните ви потребители не могат да изпращат имейли до ГД или не получават имейли от него, може да се окаже, че ГД е маркирана да позволява само имейли от вътрешни потребители.</span><span class="sxs-lookup"><span data-stu-id="d9b27-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d9b27-115">Можете да проверите тази конфигурация и да я поправите, следвайки указанията [тук](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="d9b27-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="d9b27-116">**Забележка:** Тези инструкции не важат, ако типът на групата ви е "Office 365 Group" вместо "група за разпространение".</span><span class="sxs-lookup"><span data-stu-id="d9b27-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d9b27-117">Ако случаят е такъв, можете да добавите външен потребител директно към групата от Outlook.</span><span class="sxs-lookup"><span data-stu-id="d9b27-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d9b27-118">Подробна информация за Office 365 групи гости, както и инструкции за добавяне на външни гости могат да бъдат намерени в [тази статия](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="d9b27-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  