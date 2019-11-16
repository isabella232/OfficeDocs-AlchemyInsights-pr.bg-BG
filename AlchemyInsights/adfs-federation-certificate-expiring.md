---
title: ADFS федерация сертификат изтичащ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737178"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="757f6-102">ADFS федерация сертификат изтичащ</span><span class="sxs-lookup"><span data-stu-id="757f6-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="757f6-103">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="757f6-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="757f6-104">Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако модулът вече не е инсталиран).</span><span class="sxs-lookup"><span data-stu-id="757f6-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="757f6-105">За да направите това, отидете на [управление на AZURE ad с помощта на Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="757f6-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="757f6-106">Следвайте стъпките в "сценарий 1: AD FS маркер подписване сертификат изтече" раздел на ["Възникна проблем при достъп до сайта" грешка от AD FS, когато външен потребител влезе в Office 365, Azure или InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="757f6-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="757f6-107">Следвайте стъпките в [актуализиране или поправяне на настройките на външен домейн в Office 365, Azure или InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="757f6-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="757f6-108">За да научите повече за подновяване на Федерация сертификати, вижте [подновяване федерация сертификати за Office 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="757f6-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
