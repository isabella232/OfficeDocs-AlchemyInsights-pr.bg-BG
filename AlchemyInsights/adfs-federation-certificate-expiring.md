---
title: Изтичане на срока на сертификата за федериране на ADFS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821940"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="e3e97-102">Изтичане на срока на сертификата за федериране на ADFS</span><span class="sxs-lookup"><span data-stu-id="e3e97-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="e3e97-103">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="e3e97-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="e3e97-104">Инсталирайте модула на Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът все още не е инсталиран).</span><span class="sxs-lookup"><span data-stu-id="e3e97-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="e3e97-105">За да направите това, отидете на [Управление на Azure AD с помощта на Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="e3e97-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="e3e97-106">Следвайте стъпките в раздела "Сценарий 1: Сертификатът за подписване на маркери на AD FS е изтекъл" на грешката "Възникна проблем с достъпа до сайта" от AD FS, когато федериран потребител влиза [в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="e3e97-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="e3e97-107">Следвайте стъпките в [Актуализиране или поправяне на настройките на федерирания домейн в Microsoft, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="e3e97-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="e3e97-108">За да научите повече за подновяването на сертификати за федериране, вижте Подновяване на сертификати за федериране за [Microsoft 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="e3e97-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
