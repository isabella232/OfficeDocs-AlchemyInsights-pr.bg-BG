---
title: 1048 5.7.750 услугата не е налична. Клиент, блокирани от изпращане от нерегистрирани домейни
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 5eb42679f123fcd1b680327329721cb47e18e11a
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776491"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="42128-103">5.7.750 клиент блокирани от изпращане от нерегистриран домейн</span><span class="sxs-lookup"><span data-stu-id="42128-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="42128-104">Тази грешка възниква, когато голям обем на съобщенията се изпращат от области, които не са осигурени в Office 365 (добавя като приети домейни и потвърдени).</span><span class="sxs-lookup"><span data-stu-id="42128-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="42128-105">За да избегнете тази грешка, можете да използвате сертификат базирана поща поток съединител където домейн на сертификата е осигурен, или да осигурявате всички Изпращане домейни.</span><span class="sxs-lookup"><span data-stu-id="42128-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  
