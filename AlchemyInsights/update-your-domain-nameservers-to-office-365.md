---
title: Актуализирайте своите сървъри за имена на домейните да сочат към Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510273"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="3499c-102">Актуализирайте своите сървъри за имена на домейните да сочат към Microsoft</span><span class="sxs-lookup"><span data-stu-id="3499c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="3499c-103">Забележка: За разпространението на промените в сървърите за имена понякога може да са необходими до 48 часа.</span><span class="sxs-lookup"><span data-stu-id="3499c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3499c-104">За да настроите домейна си с Microsoft, сървърните на имената на вашия регистратор трябва да бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="3499c-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="3499c-105">Създайте или редактирайте своите записи на сървърите за имена при вашия регистратор на домейни.</span><span class="sxs-lookup"><span data-stu-id="3499c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3499c-106">Отидете в уеб сайта на регистратора на домейни и намерете областта, където можете да редактирате сървърите за имена.</span><span class="sxs-lookup"><span data-stu-id="3499c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="3499c-107">Създайте или редактирайте два записа на сървърите за имена със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="3499c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3499c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3499c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3499c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3499c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3499c-110">Запишете промените.</span><span class="sxs-lookup"><span data-stu-id="3499c-110">Save changes.</span></span>

<span data-ttu-id="3499c-111">Можете да намерите подробни инструкции в тази статия: [Промяна на сървъра за имена да настроите Microsoft 365 с всеки регистратор на домейни](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="3499c-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  