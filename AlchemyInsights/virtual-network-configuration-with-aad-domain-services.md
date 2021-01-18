---
title: Виртуален конфигурационен с услуги за домейн на пад
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884858"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="975f3-102">Виртуален конфигурационен с услуги за домейн на пад</span><span class="sxs-lookup"><span data-stu-id="975f3-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="975f3-103">Виртуалното конфигуриране с услугите за домейн на пад включва следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="975f3-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="975f3-104">Проверка на изправността на вашия домейн в портала на Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="975f3-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="975f3-105">Проверяване на вашия ГЯД за правила, които блокират портове, необходими за синхронизиране в Azure AD Domain Services в портала https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="975f3-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="975f3-106">Гарантиране, че вашата виртуална мрежа е разположена в същия Azure регион като управлявания домейн на Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="975f3-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="975f3-107">Гарантиране, че нямате съществуващ домейн със същото име на домейн, което се предлага във виртуалната мрежа.</span><span class="sxs-lookup"><span data-stu-id="975f3-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="975f3-108">За повече информация относно проектните обмисляния във виртуалната мрежа на Azure за поддръжка на услугите за домейни на пад вижте [разглеждане на виртуални мрежи](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="975f3-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

