---
title: 932 надстройка AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365878"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="2becd-102">Свързване на ъпгрейд лазурно АД</span><span class="sxs-lookup"><span data-stu-id="2becd-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="2becd-103">По подразбиране автоматичен ъпгрейд е разрешена за Azure АД свържете, която помага да се гарантира, че работите най-новата версия.</span><span class="sxs-lookup"><span data-stu-id="2becd-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="2becd-104">За да проверите настройките за автоматично ъпгрейд, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure АД PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2becd-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="2becd-105">Кратката команда ще върне един от следните стойности:</span><span class="sxs-lookup"><span data-stu-id="2becd-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="2becd-106">**Активирана**: автоматичен ъпгрейд е разрешено.</span><span class="sxs-lookup"><span data-stu-id="2becd-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="2becd-107">**Забранени**: автоматичен ъпгрейд е забранено.</span><span class="sxs-lookup"><span data-stu-id="2becd-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="2becd-108">**Окачени**: системата вече има право да получава автоматично ъпгрейди.</span><span class="sxs-lookup"><span data-stu-id="2becd-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="2becd-109">Не можете да конфигурирате тази стойност; Тя се определя от системата.</span><span class="sxs-lookup"><span data-stu-id="2becd-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="2becd-110">За повече информация вижте [автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="2becd-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="2becd-111">За да изтеглите последната версия на Azure АД се свърже, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="2becd-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
