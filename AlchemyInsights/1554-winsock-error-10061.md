---
title: 1554 Winsock грешка 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903085"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="b3a37-102">Winsock грешка 10061</span><span class="sxs-lookup"><span data-stu-id="b3a37-102">Winsock error 10061</span></span>

<span data-ttu-id="b3a37-p101">Този код на грешка означава, че Office 365 не можа да установи TCP сокет (връзка) с хост. Най-вероятната причина за тази грешка е проблем с конфигурацията на защитната стена. За да коригирате проблема, проверете следните настройки:</span><span class="sxs-lookup"><span data-stu-id="b3a37-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="b3a37-106">Проверете вашата защитна стена конфигурация с информацията в [Office 365 URL и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b3a37-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="b3a37-107">Ако грешката е специфичен за Exchange онлайн защита (EOP), вие трябва да са били оповестени до промяна на [Exchange онлайн защита IP адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="b3a37-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="b3a37-108">Уверете се, че вашият интернет доставчик (ISP) не блокира пристанището.</span><span class="sxs-lookup"><span data-stu-id="b3a37-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="b3a37-109">Проверете смарт хоста и целевия сървър настройките във вашата конектори.</span><span class="sxs-lookup"><span data-stu-id="b3a37-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="b3a37-110">Обърнете внимание, че Office 365 не блокира *входящите* връзки по този начин.</span><span class="sxs-lookup"><span data-stu-id="b3a37-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

