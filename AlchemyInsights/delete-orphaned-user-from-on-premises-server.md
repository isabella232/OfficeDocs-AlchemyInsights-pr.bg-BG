---
title: Изтриване на потребител, който е сирак от локален сървър
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680124"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="1077a-102">Изтриване на потребител, който е сирак от локален сървър</span><span class="sxs-lookup"><span data-stu-id="1077a-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="1077a-103">За да премахнете потребител, който е сирак, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="1077a-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="1077a-104">Синхронизиране на форс справочен указател, като следвате инструкциите в [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="1077a-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="1077a-105">За проверка на синхронизирането на справочен указател вижте [Какво представлява хибридната самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="1077a-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="1077a-106">Ако функциите за синхронизиране са правилни, но изтриването на обекти на Active Directory не се разпространява в Azure AD, ръчно премахнете обекта сираци с помощта на един от следните модули на Azure Active Directory за кратки команди на Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1077a-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="1077a-107">Премествам-MsolContact</span><span class="sxs-lookup"><span data-stu-id="1077a-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="1077a-108">Премествам-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="1077a-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="1077a-109">Премествам-MsolUser</span><span class="sxs-lookup"><span data-stu-id="1077a-109">Remove-MsolUser</span></span>

    <span data-ttu-id="1077a-110">Например за да премахнете осиротели потребителски ИД на john.smith@contoso.com, който първоначално е създаден с помощта на синхронизиране на справочен указател, изпълнете кратката команда:</span><span class="sxs-lookup"><span data-stu-id="1077a-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="1077a-111">Remove-MsolUser-UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="1077a-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>