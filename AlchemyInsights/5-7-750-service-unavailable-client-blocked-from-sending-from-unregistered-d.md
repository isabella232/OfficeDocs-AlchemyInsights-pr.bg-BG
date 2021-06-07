---
title: 1048 5.7.750 Услугата не е налична. Клиентът е блокиран да изпраща от нерегистрирани домейни
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774240"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="dcd49-103">5.7.750 Клиентът е блокиран да изпраща от нерегистриран домейн</span><span class="sxs-lookup"><span data-stu-id="dcd49-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="dcd49-104">Грешката възниква, когато голям обем съобщения се изпращат от домейни, които не са осигурени във вашия клиент (добавени като приети домейни и проверени).</span><span class="sxs-lookup"><span data-stu-id="dcd49-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="dcd49-105">За да избегнете тази грешка, можете да използвате конектор за пощенски поток, базиран на сертификат, където домейнът на сертификата е осигурен домейн, или можете да предоставяте всички домейни за изпращане.</span><span class="sxs-lookup"><span data-stu-id="dcd49-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="dcd49-106">За повече информация вижте Коригиране на проблеми с доставянето на имейл за кодове на грешки [от 5.7.700 до 5.7.750 в Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2164955)</span><span class="sxs-lookup"><span data-stu-id="dcd49-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>