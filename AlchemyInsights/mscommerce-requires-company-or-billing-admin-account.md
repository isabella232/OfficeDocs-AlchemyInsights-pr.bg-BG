---
title: Свързване към модула на MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702604"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="f6677-102">MSCommerce изисква акаунт за фирма или администратор на фактуриране</span><span class="sxs-lookup"><span data-stu-id="f6677-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="f6677-103">Модулът MSCommerce изисква акаунт с привилегиите на администратора на фирмата или за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="f6677-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="f6677-104">Ако получите следната грешка, ще трябва да се свържете отново с различен акаунт.</span><span class="sxs-lookup"><span data-stu-id="f6677-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="f6677-105">*ErrorMessage – отдалеченият сървър върна грешка: (403) е забранена. ErrorDetails – в C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 чар: 5*</span><span class="sxs-lookup"><span data-stu-id="f6677-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="f6677-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $ _-CustomErrorMessage "Неуспешно retri...*</span><span class="sxs-lookup"><span data-stu-id="f6677-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="f6677-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="f6677-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="f6677-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="f6677-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="f6677-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. команди. WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="f6677-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="f6677-110">Ако акаунтът ви няма привилегии за администратора на фирмата или за фактуриране, обърнете се към своя ИТ администратор.</span><span class="sxs-lookup"><span data-stu-id="f6677-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
