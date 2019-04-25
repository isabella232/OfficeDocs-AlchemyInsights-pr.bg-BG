---
title: Един от вашите сертификати за услуга на локалния федерация е expiring
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419681"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="1385c-102">Един от вашите сертификати за услуга на локалния федерация е expiring</span><span class="sxs-lookup"><span data-stu-id="1385c-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="1385c-103">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="1385c-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="1385c-104">Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако вече не е инсталиран модул).</span><span class="sxs-lookup"><span data-stu-id="1385c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="1385c-105">За да направите това, отидете на [Azure Active Directory PowerShell за графика](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="1385c-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="1385c-106">Следвайте стъпките в "сценарий 1: AD FS маркер за подписване сертификат с изтекъл срок" раздел на ["Възникнал е проблем при достъпа до сайта" грешка от AD FS когато външно потребител влезе в Office 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="1385c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="1385c-107">Следвайте стъпките в т[как да актуализирате или да поправите настройките на външен домейн в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="1385c-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="1385c-108">За повече информация относно подновяване федерация сертификати вижте [подновяване на сертификат за O365 и лазурно АД](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="1385c-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

