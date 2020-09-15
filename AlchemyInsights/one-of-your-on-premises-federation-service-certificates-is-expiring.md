---
title: Изтича един от вашите локални сертификати за услуги на Федерацията
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673486"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="8d981-102">Изтича един от вашите локални сертификати за услуги на Федерацията</span><span class="sxs-lookup"><span data-stu-id="8d981-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="8d981-103">За да отстраните този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="8d981-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="8d981-104">Инсталирайте модула за Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът вече не е инсталиран).</span><span class="sxs-lookup"><span data-stu-id="8d981-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="8d981-105">За да направите това, отидете в [Azure Active Directory PowerShell за Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="8d981-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="8d981-106">Следване на стъпките в "сценарий 1: AD FS сертификатът за подписване с маркер с изтекъл срок" от ["Възникна проблем с достъпа до сайта" от AD FS, когато един външен потребител влезе в Microsoft 365, Azure или в съзвучие](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="8d981-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="8d981-107">Следвайте стъпките в [как да актуализирате или поправите настройките на външен домейн в Microsoft 365, Azure или за настройка](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="8d981-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="8d981-108">За повече информация относно подновяването на сертификатите на Федерацията вижте [подновяване на сертификат за O365 и AZURE ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="8d981-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

