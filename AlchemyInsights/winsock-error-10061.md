---
title: 1554 WinSock грешка 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698851"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="4941e-102">Winsock грешка 10061</span><span class="sxs-lookup"><span data-stu-id="4941e-102">Winsock error 10061</span></span>

<span data-ttu-id="4941e-103">Този код на грешка означава, че Microsoft не може да установи TCP сокет (връзка) с целевия хост.</span><span class="sxs-lookup"><span data-stu-id="4941e-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="4941e-104">Най-вероятната причина за тази грешка е проблем с конфигурацията на вашата защитна стена.</span><span class="sxs-lookup"><span data-stu-id="4941e-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="4941e-105">За да отстраните проблема, отметнете тези настройки:</span><span class="sxs-lookup"><span data-stu-id="4941e-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="4941e-106">Проверете конфигурацията на вашата защитна стена с информацията в [диапазони от URL и IP адреси на Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="4941e-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="4941e-107">Ако грешката е конкретна за Exchange Online Protection (EOP), трябва да сте уведомили предварително за промяна на [IP адресите за Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="4941e-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="4941e-108">Уверете се, че вашият доставчик на интернет (ISP) не блокира порта.</span><span class="sxs-lookup"><span data-stu-id="4941e-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="4941e-109">Проверете настройките за смарт хост и целеви сървър във вашите конектори.</span><span class="sxs-lookup"><span data-stu-id="4941e-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="4941e-110">Имайте предвид, че Microsoft 365 не блокира *входящите* връзки по следния начин.</span><span class="sxs-lookup"><span data-stu-id="4941e-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
