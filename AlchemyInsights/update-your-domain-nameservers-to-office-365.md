---
title: Актуализирайте вашият домейн за сървъри за имена към Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742154"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="5c8d8-102">Актуализирайте вашият домейн за сървъри за имена към Office 365</span><span class="sxs-lookup"><span data-stu-id="5c8d8-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="5c8d8-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="5c8d8-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5c8d8-104">За да настроите своя домейн в Office 365, сървърите за имена във вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="5c8d8-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="5c8d8-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="5c8d8-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5c8d8-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="5c8d8-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="5c8d8-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="5c8d8-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5c8d8-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5c8d8-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5c8d8-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5c8d8-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5c8d8-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="5c8d8-110">Save changes.</span></span>

<span data-ttu-id="5c8d8-111">Можете също да намерите подробни инструкции в тази статия. [Промяна на сървърите за имена за настройване на Office 365 с произволен регистратор на домейни](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="5c8d8-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  