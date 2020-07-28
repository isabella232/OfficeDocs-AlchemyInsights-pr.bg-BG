---
title: Не може да се промени потребителско име
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438785"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="849f0-102">Не може да се промени потребителско име</span><span class="sxs-lookup"><span data-stu-id="849f0-102">Unable to change UserName</span></span>

<span data-ttu-id="849f0-103">В някои случаи UPN (UserPrincipalName) промени не се разпространяват в облака.</span><span class="sxs-lookup"><span data-stu-id="849f0-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="849f0-104">Може да получите грешки при проверка в портала на Office 365 или да не можете да промените потребителското име или имейл адреса.</span><span class="sxs-lookup"><span data-stu-id="849f0-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="849f0-105">За да разрешите този проблем, ръчно задайте UserPrincipalName с помощта на тази команда PowerShell .</span><span class="sxs-lookup"><span data-stu-id="849f0-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="849f0-106">**Пример: Преименуване на потребител**</span><span class="sxs-lookup"><span data-stu-id="849f0-106">**Example: Rename a user**</span></span>

<span data-ttu-id="849f0-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="849f0-107">PowerShellCopy</span></span>

<span data-ttu-id="849f0-108">PS C: \> Задайте MsolUserPrincipalName - Потребителско име на потребителя "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="849f0-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="849f0-109">Тази команда преименува davidc@contoso.com на davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="849f0-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="849f0-110">За повече информация вижте [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="849f0-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>