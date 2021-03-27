---
title: Ръчно влизане в Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398646"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="fd02b-102">Ръчно влизане в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fd02b-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="fd02b-103">Ако потребителят не е влизал автоматично по време на първото изпълнение, потребителят може ръчно да влезете в настройките на браузъра или в менюто за самоличност.</span><span class="sxs-lookup"><span data-stu-id="fd02b-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="fd02b-104">За да управлявате влизането, използвайте следните правила:</span><span class="sxs-lookup"><span data-stu-id="fd02b-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="fd02b-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – За да сте сигурни, че потребителят винаги има работен профил в Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="fd02b-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="fd02b-106">[Ограничаване наSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – За да ограничите влизането до набор от надеждни акаунти.</span><span class="sxs-lookup"><span data-stu-id="fd02b-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="fd02b-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – За да забраните влизането или да накарате потребителите да впишат.</span><span class="sxs-lookup"><span data-stu-id="fd02b-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

