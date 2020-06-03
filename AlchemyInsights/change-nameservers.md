---
title: Промяна на NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508077"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="e1e9a-102">Актуализирайте своите сървъри за имена на домейните да сочат към Microsoft</span><span class="sxs-lookup"><span data-stu-id="e1e9a-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="e1e9a-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="e1e9a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e1e9a-104">За да настроите своя домейн в Microsoft 365, сървърите за имена във вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="e1e9a-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e1e9a-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="e1e9a-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e1e9a-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="e1e9a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e1e9a-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="e1e9a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e1e9a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e1e9a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e1e9a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e1e9a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e1e9a-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="e1e9a-110">Save changes.</span></span>

<span data-ttu-id="e1e9a-111">Можете също да намерите подробни инструкции в тази статия. [Промяна на сървърите за имена с произволен регистратор на домейни](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="e1e9a-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  