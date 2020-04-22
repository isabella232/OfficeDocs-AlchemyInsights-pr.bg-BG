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
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706744"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="899d6-102">Актуализирайте своите сървъри за имена на домейните да сочат към Microsoft</span><span class="sxs-lookup"><span data-stu-id="899d6-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="899d6-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="899d6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="899d6-104">За да настроите своя домейн в Microsoft 365, сървърите за имена във вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="899d6-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="899d6-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="899d6-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="899d6-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="899d6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="899d6-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="899d6-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="899d6-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="899d6-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="899d6-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="899d6-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="899d6-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="899d6-110">Save changes.</span></span>

<span data-ttu-id="899d6-111">Можете също да намерите подробни инструкции в тази статия. [Промяна на сървърите за имена с произволен регистратор на домейни](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="899d6-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  