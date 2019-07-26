---
title: Промяна на NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902918"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="d6026-102">Актуализирайте вашият домейн за сървъри за имена към Office 365</span><span class="sxs-lookup"><span data-stu-id="d6026-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="d6026-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="d6026-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="d6026-104">За да настроите своя домейн в Office 365, сървърите за имена във вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="d6026-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="d6026-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="d6026-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="d6026-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="d6026-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="d6026-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="d6026-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="d6026-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d6026-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="d6026-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d6026-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="d6026-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="d6026-110">Save changes.</span></span>

<span data-ttu-id="d6026-111">Можете също да намерите подробни инструкции в тази статия. [Промяна на сървърите за имена за настройване на Office 365 с произволен регистратор на домейни](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="d6026-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  