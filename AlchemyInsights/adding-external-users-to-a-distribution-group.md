---
title: Добавяне на външни потребители към група за разпространение
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910921"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="79dea-102">Добавяне на външни потребители към група за разпространение</span><span class="sxs-lookup"><span data-stu-id="79dea-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="79dea-103">Добавянето на външен контакт към група за разпространение е процес от две стъпки:</span><span class="sxs-lookup"><span data-stu-id="79dea-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="79dea-104">Създаване на контакт за поща за външни потребители:</span><span class="sxs-lookup"><span data-stu-id="79dea-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="79dea-105">В центъра за администриране отидете на страницата с **Users**  >  [Контакти](https://admin.microsoft.com/adminportal/home#/Contact) на потребителите.</span><span class="sxs-lookup"><span data-stu-id="79dea-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="79dea-106">Изберете **Добавяне на контакт**.</span><span class="sxs-lookup"><span data-stu-id="79dea-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="79dea-107">Въведете информацията за вашия контакт и изберете **Добави**.</span><span class="sxs-lookup"><span data-stu-id="79dea-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="79dea-108">Добавете контакта за поща към вашата ГД:</span><span class="sxs-lookup"><span data-stu-id="79dea-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="79dea-109">В центъра за администриране отидете на страницата **Groups**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="79dea-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="79dea-110">Намерете Генералната дирекция, към която искате да добавите външния потребител, и я изберете, за да отворите диалоговия прозорец "Редактиране".</span><span class="sxs-lookup"><span data-stu-id="79dea-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="79dea-111">В раздела **членове** изберете **Преглед на всички и управление на членовете**.</span><span class="sxs-lookup"><span data-stu-id="79dea-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="79dea-112">Изберете **Добавяне на членове**.</span><span class="sxs-lookup"><span data-stu-id="79dea-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="79dea-113">Изберете контакта за поща, който създадохте в предишната стъпка, и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="79dea-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="79dea-114">Ако след като изпълните тези стъпки, външните потребители не могат да изпращат имейли до ГД или да не получават имейли от нея, може да се окаже, че Генералната дирекция е маркирана да позволява имейли само от вътрешни потребители.</span><span class="sxs-lookup"><span data-stu-id="79dea-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="79dea-115">Можете да проверите тази конфигурация и да я коригирате, като следвате инструкциите [тук](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="79dea-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="79dea-116">**Забележка:** Тези инструкции не важат, ако типът на групата ви е "Microsoft 365 Group" вместо "група за разпространение".</span><span class="sxs-lookup"><span data-stu-id="79dea-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="79dea-117">Ако това е така, можете да добавите външния потребител директно към групата от Outlook.</span><span class="sxs-lookup"><span data-stu-id="79dea-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="79dea-118">Подробна информация за гостите на Microsoft 365 Groups, както и инструкции за добавяне на външни гости, могат да бъдат намерени в [тази статия](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="79dea-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  