---
title: Как да добавите или премахнете представител в Outlook за Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573303"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="3b39d-102">Как да добавите или премахнете представител в Outlook за Windows</span><span class="sxs-lookup"><span data-stu-id="3b39d-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="3b39d-103">За да добавите представител в Outlook за Windows:</span><span class="sxs-lookup"><span data-stu-id="3b39d-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="3b39d-104">Щракнете върху раздела **файл** , последван от **Настройки на акаунт**, и след това изберете **делегиране на достъп**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="3b39d-105">Щракнете върху **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-105">Click on **Add**.</span></span> <span data-ttu-id="3b39d-106">Ако **Add** не се показва, е възможно да не съществува активна връзка между Outlook и Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b39d-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="3b39d-107">Лентата на състоянието на Outlook показва състоянието на връзката.</span><span class="sxs-lookup"><span data-stu-id="3b39d-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="3b39d-108">Въведете името на човека, когото искате да посочите като ваш представител, или потърсете и изберете името от списъка с резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="3b39d-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3b39d-109">Представителят трябва да е лице, което е в глобалния адресен списък на Exchange на вашата организация (GAL).</span><span class="sxs-lookup"><span data-stu-id="3b39d-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="3b39d-110">Щракнете върху **Добавяне** , последвано от **OK**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="3b39d-111">В диалоговия прозорец **делегиране на разрешения** приемете настройките по подразбиране за разрешения или изберете нива на достъп по избор за папките на Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b39d-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="3b39d-112">Ако един представител има нужда от разрешение за работа само с искания за събрания и отговори, настройките по подразбиране за разрешения, като например **делегат, получава копия на съобщения, свързани със събрания, изпратени до мен** , са достатъчни.</span><span class="sxs-lookup"><span data-stu-id="3b39d-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="3b39d-113">Можете да оставите настройката за разрешение **"Входящи" на "** **няма**".</span><span class="sxs-lookup"><span data-stu-id="3b39d-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="3b39d-114">Исканията за събрания и отговорите ще отиват директно към папката "Входящи" на представителя.</span><span class="sxs-lookup"><span data-stu-id="3b39d-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3b39d-115">По подразбиране представителят е отпуснал разрешение за **Редактиране, създаване и промяна на елементи** в папката " **Календар** ".</span><span class="sxs-lookup"><span data-stu-id="3b39d-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="3b39d-116">Когато Делегатът отговаря на събрание от ваше име, то се добавя автоматично към папката на **календара** ви.</span><span class="sxs-lookup"><span data-stu-id="3b39d-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="3b39d-117">За да изпратите съобщение за уведомяване на представителя за променените разрешения, поставете отметка в квадратчето **автоматично Изпращай на представителя съобщение, обобщаващо тези разрешения** .</span><span class="sxs-lookup"><span data-stu-id="3b39d-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="3b39d-118">Ако искате, изберете квадратчето за отметка **Представителят може да вижда моята поверителна** информация.</span><span class="sxs-lookup"><span data-stu-id="3b39d-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="3b39d-119">Тази настройка засяга всички папки на Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b39d-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="3b39d-120">Това включва всички съобщения, контакти, календар, задачи, бележки и папки за дневници.</span><span class="sxs-lookup"><span data-stu-id="3b39d-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="3b39d-121">Няма начин да дадете достъп до поверителните елементи само в определени папки.</span><span class="sxs-lookup"><span data-stu-id="3b39d-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="3b39d-122">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="3b39d-123">Съобщения, изпратени чрез разрешения за изпращане от името на представителя, включват и имената на представителите и вашите имена до **от**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="3b39d-124">Когато съобщението бъде изпратено с разрешения "Изпращане като", се показва само вашето име.</span><span class="sxs-lookup"><span data-stu-id="3b39d-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="3b39d-125">След като добавите някого като представител, той може да добави вашата пощенска кутия на Exchange към своя профил в Outlook.</span><span class="sxs-lookup"><span data-stu-id="3b39d-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="3b39d-126">За инструкции вижте [управление на пощенските съобщения и календарните елементи на друг човек](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="3b39d-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="3b39d-127">За да премахнете представител в Outlook за Windows:</span><span class="sxs-lookup"><span data-stu-id="3b39d-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="3b39d-128">Щракнете върху раздела **файл** .</span><span class="sxs-lookup"><span data-stu-id="3b39d-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="3b39d-129">Щракнете върху **Настройки на акаунт** , последвани от **делегиран достъп**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="3b39d-130">Изберете името на представителя, за когото искате да промените разрешенията, и след това щракнете върху **Премахни** , последвано от **OK**.</span><span class="sxs-lookup"><span data-stu-id="3b39d-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
