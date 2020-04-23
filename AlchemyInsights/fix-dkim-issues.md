---
title: Отстраняване на проблеми с dKIM настройка
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717551"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="ba7e5-102">Отстраняване на проблеми с dKIM настройка</span><span class="sxs-lookup"><span data-stu-id="ba7e5-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="ba7e5-103">Ако имате проблеми, позволяващи DKIM за вашия домейн, използвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="ba7e5-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="ba7e5-104">Повечето DKIM настройка проблеми са свързани с неправилни DNS записи.</span><span class="sxs-lookup"><span data-stu-id="ba7e5-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="ba7e5-105">Проверете DKIM CNAME запис **(не** TXT запис) е форматиран правилно.</span><span class="sxs-lookup"><span data-stu-id="ba7e5-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="ba7e5-106">За повече информация вижте тази [тема](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="ba7e5-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="ba7e5-107">След като създадете или актуализирате DKIM DNS записи в DNS хостинг услуга за вашия домейн (обикновено, вашия домейн регистратор), изчакайте DNS записите да се разпространяват.</span><span class="sxs-lookup"><span data-stu-id="ba7e5-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="ba7e5-108">Ако не можете да създадете DKIM DNS записи в \<центъра\> за администриране, можете да замените CustomDomain с вашия потребителски `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`домейн (например contoso.com) и изпълнете тази команда в Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .</span><span class="sxs-lookup"><span data-stu-id="ba7e5-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
