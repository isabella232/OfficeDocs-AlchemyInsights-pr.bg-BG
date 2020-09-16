---
title: Промяна на NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714677"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="a88aa-102">Актуализирайте своите сървъри за имена на домейните да сочат към Microsoft</span><span class="sxs-lookup"><span data-stu-id="a88aa-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="a88aa-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="a88aa-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a88aa-104">За да настроите своя домейн в Microsoft 365, сървърите за имена във вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="a88aa-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="a88aa-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="a88aa-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a88aa-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="a88aa-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="a88aa-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="a88aa-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="a88aa-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a88aa-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="a88aa-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a88aa-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="a88aa-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="a88aa-110">Save changes.</span></span>

<span data-ttu-id="a88aa-111">Можете също да намерите подробни инструкции в тази статия. [Промяна на сървърите за имена с произволен регистратор на домейни](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="a88aa-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  