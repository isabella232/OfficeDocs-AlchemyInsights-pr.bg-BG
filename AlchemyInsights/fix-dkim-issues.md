---
title: Отстраняване на проблеми при настройване на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506763"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="c9749-102">Отстраняване на проблеми при настройване на DKIM</span><span class="sxs-lookup"><span data-stu-id="c9749-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="c9749-103">Ако имате проблеми с DKIM за вашия домейн, използвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="c9749-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="c9749-104">Повечето DKIM настройка проблеми са свързани с неправилни DNS записи.</span><span class="sxs-lookup"><span data-stu-id="c9749-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="c9749-105">Проверете DKIM CNAME запис **(не** TXT запис) е форматиран правилно.</span><span class="sxs-lookup"><span data-stu-id="c9749-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="c9749-106">За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="c9749-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="c9749-107">След като създадете или актуализирате DKIM DNS записи в DNS хостинг услугата за вашия домейн (обикновено, вашия регистратор на домейни), изчакайте DNS записи да се разпространяват.</span><span class="sxs-lookup"><span data-stu-id="c9749-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="c9749-108">Ако не можете да създадете DKIM DNS записи в центъра за администриране, можете да \<CustomDomain\> замените с вашия потребителски домейн (например contoso.com) и да изпълните тази команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="c9749-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
