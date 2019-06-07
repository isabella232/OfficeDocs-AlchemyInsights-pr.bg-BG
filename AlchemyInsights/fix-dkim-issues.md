---
title: Прикрепвам проблеми с инсталирането на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764845"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="f9099-102">Прикрепвам проблеми с инсталирането на DKIM</span><span class="sxs-lookup"><span data-stu-id="f9099-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="f9099-103">Ако имате въпроси, позволяващи DKIM за потребителски домейна, използвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="f9099-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="f9099-104">Повечето DKIM настройка проблеми са свързани с неправилен DNS записи.</span><span class="sxs-lookup"><span data-stu-id="f9099-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="f9099-105">Проверете DKIM CNAME запис (**не** TXT запис) е форматиран правилно.</span><span class="sxs-lookup"><span data-stu-id="f9099-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="f9099-106">За повече информация вижте тази [тема](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f9099-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="f9099-107">След като създадете или актуализирате вашите DKIM DNS записи в услугата за DNS хостинг за вашия домейн (обикновено вашия регистратор на домейн), изчакайте за DNS, записите да пропагандира.</span><span class="sxs-lookup"><span data-stu-id="f9099-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="f9099-108">Ако не може да създадете DKIM DNS записи в центъра на администратор, можете да замените \<CustomDomain\> с вашия собствен домейн (например contoso.com) и стартирате тази команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="f9099-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
