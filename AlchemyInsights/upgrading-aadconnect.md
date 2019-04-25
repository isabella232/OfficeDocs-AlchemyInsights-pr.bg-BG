---
title: 932 надстройка AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389648"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="34c48-102">Свързване на ъпгрейд лазурно АД</span><span class="sxs-lookup"><span data-stu-id="34c48-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="34c48-103">По подразбиране автоматичен ъпгрейд е разрешена за Azure АД свържете, която помага да се гарантира, че работите най-новата версия.</span><span class="sxs-lookup"><span data-stu-id="34c48-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="34c48-104">За да проверите настройките за автоматично ъпгрейд, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure АД PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34c48-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="34c48-105">Кратката команда ще върне един от следните стойности:</span><span class="sxs-lookup"><span data-stu-id="34c48-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="34c48-106">**Активирана**: автоматичен ъпгрейд е разрешено.</span><span class="sxs-lookup"><span data-stu-id="34c48-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="34c48-107">**Забранени**: автоматичен ъпгрейд е забранено.</span><span class="sxs-lookup"><span data-stu-id="34c48-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="34c48-108">**Окачени**: системата вече има право да получава автоматично ъпгрейди.</span><span class="sxs-lookup"><span data-stu-id="34c48-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="34c48-109">Не можете да конфигурирате тази стойност; Тя се определя от системата.</span><span class="sxs-lookup"><span data-stu-id="34c48-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="34c48-110">За повече информация вижте [автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="34c48-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="34c48-111">За да изтеглите последната версия на Azure АД се свърже, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="34c48-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
