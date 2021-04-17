---
title: Отстраняване на неизправности с съвета за безопасност за проверки за откриване на измами
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834720"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="fb6bc-102">Отстраняване на неизправности с съвета за безопасност за проверки за откриване на измами</span><span class="sxs-lookup"><span data-stu-id="fb6bc-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="fb6bc-103">Ако получавате съвет за безопасност, който гласи "Подателят не е изпълнил нашите проверки за откриване на измами и може да не е този, който изглежда, че е", тогава подателят не е преминал проверки за удостоверяване на DKIM или SPF.</span><span class="sxs-lookup"><span data-stu-id="fb6bc-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="fb6bc-104">Най-добрият метод за разрешаване на проблема е подателят да се оторизира.</span><span class="sxs-lookup"><span data-stu-id="fb6bc-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="fb6bc-105">Ако подателят изпраща от ваше име, трябва да го оторизирате, като добавите IP адреса на подателя към вашия SPF запис.</span><span class="sxs-lookup"><span data-stu-id="fb6bc-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="fb6bc-106">Вижте [Отстраняване на неизправности с червения (подозрителен) съвет за безопасност за проверки за откриване на](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) измами за повече информация.</span><span class="sxs-lookup"><span data-stu-id="fb6bc-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="fb6bc-107">Ето някои други връзки, които могат да ви помогнат:</span><span class="sxs-lookup"><span data-stu-id="fb6bc-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="fb6bc-108">Как Microsoft използва рамката за правила за податели (SPF), за да предотврати подсказка</span><span class="sxs-lookup"><span data-stu-id="fb6bc-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="fb6bc-109">Настройване на SPF за предотвратяване на подпухване</span><span class="sxs-lookup"><span data-stu-id="fb6bc-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
