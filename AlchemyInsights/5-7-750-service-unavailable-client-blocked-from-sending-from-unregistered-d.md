---
title: услугата 1048 5.7.750 е недостъпна. Клиентът е блокиран от изпращането на нерегистрирани домейни
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
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664231"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="284a1-103">клиент на 5.7.750 е блокиран от изпращането на нерегистриран домейн</span><span class="sxs-lookup"><span data-stu-id="284a1-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="284a1-104">Грешката възниква, когато голям обем съобщения се изпращат от домейни, които не са осигурени във вашия клиент (добавени като приети домейни и утвърдени).</span><span class="sxs-lookup"><span data-stu-id="284a1-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="284a1-105">За да избегнете тази грешка, можете да използвате базиран на сертификат конектор за пощенски поток, в който домейнът на сертификата е осигуряващ домейн, или можете да осигурите всички изпращащи домейни.</span><span class="sxs-lookup"><span data-stu-id="284a1-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
