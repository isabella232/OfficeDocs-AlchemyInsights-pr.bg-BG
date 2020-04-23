---
title: Отстраняване на неизправности в накрайника за безопасност при проверки за откриване на измами
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759501"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="22c8c-102">Отстраняване на неизправности в накрайника за безопасност при проверки за откриване на измами</span><span class="sxs-lookup"><span data-stu-id="22c8c-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="22c8c-103">Ако получавате съвет за безопасност, който казва "Подателят не успя да провери за откриване на измами и може да не е това, което изглежда да е", тогава подателят не успя да премине DKIM или SPF проверка за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="22c8c-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="22c8c-104">Най-добрият начин за разрешаване на това е подателят да се оторизира.</span><span class="sxs-lookup"><span data-stu-id="22c8c-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="22c8c-105">Ако изпращащия от Ваше име, трябва да ги упълномощите, като добавите IP адреса на подателя към вашия SPF запис.</span><span class="sxs-lookup"><span data-stu-id="22c8c-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="22c8c-106">Вижте [Отстраняване на неизправности с червения (подозрителен) съвет за проверка за откриване на измами](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="22c8c-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="22c8c-107">Ето някои други връзки, които могат да помогнат:</span><span class="sxs-lookup"><span data-stu-id="22c8c-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="22c8c-108">Как Microsoft използва рамка за правила на подателя (SPF) за предотвратяване на подслона</span><span class="sxs-lookup"><span data-stu-id="22c8c-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="22c8c-109">Настройване на SPF, за да се предотврати подслона</span><span class="sxs-lookup"><span data-stu-id="22c8c-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
