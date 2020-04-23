---
title: 1554 Winsock грешка 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766158"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="67ee2-102">Winsock грешка 10061</span><span class="sxs-lookup"><span data-stu-id="67ee2-102">Winsock error 10061</span></span>

<span data-ttu-id="67ee2-103">Този код на грешка означава, че Microsoft не може да установи TCP гнездо (връзка) с целеви хост.</span><span class="sxs-lookup"><span data-stu-id="67ee2-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="67ee2-104">Най-вероятната причина за тази грешка е проблемът с конфигурацията на защитната стена.</span><span class="sxs-lookup"><span data-stu-id="67ee2-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="67ee2-105">За да отстраните проблема, проверете следните настройки:</span><span class="sxs-lookup"><span data-stu-id="67ee2-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="67ee2-106">Проверете конфигурацията на защитната стена с информацията в [URL адреси темпота на Microsoft 365 и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="67ee2-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="67ee2-107">Ако грешката е специфична за Exchange Online Protection (EOP), трябва предварително да са били уведомени за промяна на [Ip адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)те .</span><span class="sxs-lookup"><span data-stu-id="67ee2-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="67ee2-108">Проверете дали интернет доставчикът не блокира порта.</span><span class="sxs-lookup"><span data-stu-id="67ee2-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="67ee2-109">Проверете интелигентния хост и целевите настройки на сървъра във вашите конектори.</span><span class="sxs-lookup"><span data-stu-id="67ee2-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="67ee2-110">Имайте предвид, че Microsoft 365 не блокира *входящите* връзки по този начин.</span><span class="sxs-lookup"><span data-stu-id="67ee2-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
