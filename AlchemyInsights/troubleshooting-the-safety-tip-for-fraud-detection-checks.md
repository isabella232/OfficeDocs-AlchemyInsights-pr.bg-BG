---
title: Съвет за безопасност за разкриването на измами за отстраняване на неизправности проверява
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353238"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="9ca50-102">Съвет за безопасност за разкриването на измами за отстраняване на неизправности проверява</span><span class="sxs-lookup"><span data-stu-id="9ca50-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="9ca50-103">Ако сте получаване на безопасност върха, че се казва "подателя неуспешно проверки за откриване ни измами и може да не е кой те изглеждат", след което подателят не успя да премине DKIM или SPF удостоверяване проверки.</span><span class="sxs-lookup"><span data-stu-id="9ca50-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="9ca50-104">Най-добрият метод за решаване на това е за подателя да разрешат сами.</span><span class="sxs-lookup"><span data-stu-id="9ca50-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="9ca50-105">Ако подателят изпраща от ваше име, трябва да ги разрешат чрез добавяне на IP адреса на подателя към вашия SPF запис.</span><span class="sxs-lookup"><span data-stu-id="9ca50-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="9ca50-106">Вижте [отстраняване на червено (подозрителни) безопасност съвет за разкриване на измами проверява](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="9ca50-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="9ca50-107">Ето някои други връзки, които могат да помогнат:</span><span class="sxs-lookup"><span data-stu-id="9ca50-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="9ca50-108">Как Office 365 използва изпращам политика рамки (SPF), за да предотврати измама</span><span class="sxs-lookup"><span data-stu-id="9ca50-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="9ca50-109">Поставям горе SPF в Office 365 за предпазване от изигравам</span><span class="sxs-lookup"><span data-stu-id="9ca50-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
