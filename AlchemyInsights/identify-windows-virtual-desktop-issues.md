---
title: Идентифициране на проблеми с виртуалния работен плот на Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595456"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="7dee7-102">Идентифициране на проблеми с виртуалния работен плот на Windows</span><span class="sxs-lookup"><span data-stu-id="7dee7-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="7dee7-103">Диагностиката на виртуалния работен плот на Windows използва само една кратка команда на PowerShell, но съдържа много незадължителни параметри, за да ви помогне да стесните и изолирате проблемите.</span><span class="sxs-lookup"><span data-stu-id="7dee7-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="7dee7-104">За да започнете:</span><span class="sxs-lookup"><span data-stu-id="7dee7-104">To get started:</span></span> 

1. <span data-ttu-id="7dee7-105">Изтеглете и импортирайте модула на Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7dee7-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="7dee7-106">За подробности вижте Кратки команди [за виртуален работен плот на Windows за Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="7dee7-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="7dee7-107">Изпълнете следната кратка команда, за да влезете в акаунта си:</span><span class="sxs-lookup"><span data-stu-id="7dee7-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="7dee7-108">Пример: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="7dee7-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="7dee7-109">**ЗАБЕЛЕЖКА:** Всички заявки, използващи PowerShell, трябва да включват параметрите -UserName или -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="7dee7-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="7dee7-110">За възможности за наблюдение вижте Използване [на log Analytics за функцията за диагностика](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="7dee7-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="7dee7-111">За да филтрирате диагностичните дейности по потребител, изпълнете следната кратка команда:</span><span class="sxs-lookup"><span data-stu-id="7dee7-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="7dee7-112">Пример: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="7dee7-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="7dee7-113">Има списък с филтри, които можете да изпълните, за да диагностицирате проблеми.</span><span class="sxs-lookup"><span data-stu-id="7dee7-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="7dee7-114">За да научите повече за диагностицирането на проблеми, вижте [Идентифициране и диагностициране на проблеми с виртуалния работен плот на Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="7dee7-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="7dee7-115">За да научите повече за често срещаните грешки, вижте [Често срещани грешки senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="7dee7-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
