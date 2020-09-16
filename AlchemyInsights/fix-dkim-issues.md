---
title: Отстраняване на проблеми с настройката на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744939"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="98a26-102">Отстраняване на проблеми с настройката на DKIM</span><span class="sxs-lookup"><span data-stu-id="98a26-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="98a26-103">Ако имате проблеми с активирането на DKIM за вашия домейн по избор, използвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="98a26-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="98a26-104">Повечето проблеми при настройването на DKIM се отнасят за неправилни DNS записи.</span><span class="sxs-lookup"><span data-stu-id="98a26-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="98a26-105">Проверете дали CNAME записът за DKIM (**не** е TXT запис) е форматиран правилно.</span><span class="sxs-lookup"><span data-stu-id="98a26-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="98a26-106">За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="98a26-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="98a26-107">След като създадете или актуализирате вашите DNS записи за DKIM в услугата за DNS хостинг за вашия домейн (обикновено регистратор на домейни), изчакайте DNS записите да се разпространят.</span><span class="sxs-lookup"><span data-stu-id="98a26-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="98a26-108">Ако не можете да създадете DKIM DNS Records в центъра за администриране, можете да заместите \<CustomDomain\> с вашия домейн по избор (например contoso.com) и да изпълните тази команда в [PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="98a26-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
