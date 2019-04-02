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
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772431"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="fffc3-102">Winsock грешка 10061</span><span class="sxs-lookup"><span data-stu-id="fffc3-102">Winsock error 10061</span></span>

<span data-ttu-id="fffc3-103">Този код на грешка означава, че Office 365 не можа да установи TCP сокет (връзка) с хост.</span><span class="sxs-lookup"><span data-stu-id="fffc3-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="fffc3-104">Най-вероятната причина за тази грешка е проблем с конфигурацията на защитната стена.</span><span class="sxs-lookup"><span data-stu-id="fffc3-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="fffc3-105">За да коригирате проблема, проверете следните настройки:</span><span class="sxs-lookup"><span data-stu-id="fffc3-105">To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="fffc3-106">Проверете вашата защитна стена конфигурация с информацията в [Office 365 URL и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="fffc3-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="fffc3-107">Ако грешката е специфичен за Exchange онлайн защита (EOP), вие трябва да са били оповестени до промяна на [Exchange онлайн защита IP адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="fffc3-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="fffc3-108">Уверете се, че вашият интернет доставчик (ISP) не блокира пристанището.</span><span class="sxs-lookup"><span data-stu-id="fffc3-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="fffc3-109">Проверете смарт хоста и целевия сървър настройките във вашата конектори.</span><span class="sxs-lookup"><span data-stu-id="fffc3-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="fffc3-110">Обърнете внимание, че Office 365 не блокира *входящите* връзки по този начин.</span><span class="sxs-lookup"><span data-stu-id="fffc3-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  
