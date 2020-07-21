---
title: Изтриване на осиротели потребител от локалния сървър
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197821"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="2c8c4-102">Изтриване на осиротели потребител от локалния сървър</span><span class="sxs-lookup"><span data-stu-id="2c8c4-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="2c8c4-103">За да премахнете загубен потребител, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="2c8c4-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="2c8c4-104">Сила на указатели, като следвате инструкциите в [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="2c8c4-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="2c8c4-105">За да проверите синхронизирането на директории, вижте [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="2c8c4-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="2c8c4-106">Ако синхронизиране функционира правилно, но изтриване на active Directory обект не се разпространява azure AD, ръчно премахнете очесящи обект чрез един от следните Azure Active Directory модул за кратки команди на Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2c8c4-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="2c8c4-107">Премахване на MsolConContact</span><span class="sxs-lookup"><span data-stu-id="2c8c4-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="2c8c4-108">Премахване на MsolGroup</span><span class="sxs-lookup"><span data-stu-id="2c8c4-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="2c8c4-109">Премахване на MsolUser</span><span class="sxs-lookup"><span data-stu-id="2c8c4-109">Remove-MsolUser</span></span>

    <span data-ttu-id="2c8c4-110">Например да премахнете осиротели потребителски ИД john.smith@contoso.com, първоначално създаден чрез синхронизиране на директории, изпълнете команда:</span><span class="sxs-lookup"><span data-stu-id="2c8c4-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="2c8c4-111">Премахване на MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="2c8c4-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>