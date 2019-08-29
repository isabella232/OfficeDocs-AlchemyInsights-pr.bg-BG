---
title: Добавяне на външни потребители до група за разпространение
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660781"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="ce3ff-102">Добавяне на външни потребители до група за разпространение</span><span class="sxs-lookup"><span data-stu-id="ce3ff-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="ce3ff-103">Добавянето на външен контакт към група разпространение (ГД) е двуетапен процес:</span><span class="sxs-lookup"><span data-stu-id="ce3ff-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="ce3ff-104">Създаване на контакт за поща за външен потребител:</span><span class="sxs-lookup"><span data-stu-id="ce3ff-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="ce3ff-105">В центъра на администратор, отидете на **потребителите** > [Контакти](https://admin.microsoft.com/adminportal/home#/Contact) страница.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="ce3ff-106">Изберете **Добави контакт**.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="ce3ff-107">Въведете информацията за вашия контакт и изберете **добав**.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="ce3ff-108">Добавете контакт за поща към вашия ГД:</span><span class="sxs-lookup"><span data-stu-id="ce3ff-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="ce3ff-109">В центъра на администратор, отидете на **групи** > страница[групи](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="ce3ff-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="ce3ff-110">Намерете ГД, който искате да добавите външен потребител и изберете да отворите диалоговия прозорец за редактиране.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="ce3ff-111">В раздела на **членовете** изберете **Покажи всички и управление на членове**.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="ce3ff-112">Изберете **Добавяне на членове**.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="ce3ff-113">Изберете контакт за поща, създадохте в предишната стъпка и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="ce3ff-114">Ако след последователи тези стъпвам вашите външни потребители не могат да изпращат имейли до ГД или не получавате имейли от него, тя може да бъде, че ГД е маркиран, за да позволяват само имейли от вътрешни потребители.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="ce3ff-115">Можете да проверите тази конфигурация и прикрепвам то следвате указанията [тук](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce3ff-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="ce3ff-116">**Забележка:** Тези указания не се прилагат, ако типът на вашата група е "Office 365 група" а "Група за разпространение."</span><span class="sxs-lookup"><span data-stu-id="ce3ff-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="ce3ff-117">Ако случаят е такъв, можете да добавите външен потребител директно към групата от Outlook.</span><span class="sxs-lookup"><span data-stu-id="ce3ff-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="ce3ff-118">Подробна информация за Office 365 групи увреждания, както и инструкции за добавяне на външни увреждания могат да бъдат намерени в [тази статия](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce3ff-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  