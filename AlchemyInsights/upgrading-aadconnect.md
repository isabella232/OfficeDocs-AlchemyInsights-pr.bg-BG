---
title: 932 надстройване на AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806028"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="3f340-102">Надстройка на Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3f340-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="3f340-103">По подразбиране автоматичната надстройка е разрешена за Azure AD Connect, което ще ви помогне да се уверите, че използвате най-новата версия.</span><span class="sxs-lookup"><span data-stu-id="3f340-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="3f340-104">За да проверите настройките за автоматично надстройване, използвайте кратката команда **get-ADSyncAutoUpgrade** в Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3f340-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="3f340-105">Кратката команда ще върне една от следните стойности:</span><span class="sxs-lookup"><span data-stu-id="3f340-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="3f340-106">**Разрешена**: автоматичната надстройка е разрешена.</span><span class="sxs-lookup"><span data-stu-id="3f340-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="3f340-107">**Изключен**: автоматичната надстройка е забранена.</span><span class="sxs-lookup"><span data-stu-id="3f340-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="3f340-108">**Спряно**: системата вече не отговаря на условията за получаване на автоматични надстройки.</span><span class="sxs-lookup"><span data-stu-id="3f340-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="3f340-109">Не можете да конфигурирате тази стойност; Това е зададено от системата.</span><span class="sxs-lookup"><span data-stu-id="3f340-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="3f340-110">За повече информация вижте [автоматично надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="3f340-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="3f340-111">За да изтеглите най-новата версия на Azure AD Connect, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="3f340-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
