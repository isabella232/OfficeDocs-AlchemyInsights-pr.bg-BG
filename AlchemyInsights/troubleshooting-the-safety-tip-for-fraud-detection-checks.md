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
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658104"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="0cb87-102">Съвет за безопасност за разкриването на измами за отстраняване на неизправности проверява</span><span class="sxs-lookup"><span data-stu-id="0cb87-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="0cb87-p101">Ако сте получаване на безопасност върха, че се казва "подателя неуспешно проверки за откриване ни измами и може да не е кой те изглеждат", след което подателят не успя да премине DKIM или SPF удостоверяване проверки. Най-добрият метод за решаване на това е за подателя да разрешат сами. Ако подателят изпраща от ваше име, трябва да ги разрешат чрез добавяне на IP адреса на подателя към вашия SPF запис.</span><span class="sxs-lookup"><span data-stu-id="0cb87-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="0cb87-106">Вижте [отстраняване на червено (подозрителни) безопасност съвет за разкриване на измами проверява](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="0cb87-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="0cb87-107">Ето някои други връзки, които могат да помогнат:</span><span class="sxs-lookup"><span data-stu-id="0cb87-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="0cb87-108">Как Office 365 използва изпращам политика рамки (SPF), за да предотврати измама</span><span class="sxs-lookup"><span data-stu-id="0cb87-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="0cb87-109">Поставям горе SPF в Office 365 за предпазване от изигравам</span><span class="sxs-lookup"><span data-stu-id="0cb87-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

