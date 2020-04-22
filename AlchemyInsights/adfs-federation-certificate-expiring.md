---
title: Adfs федерация сертификат с изтекъл срок
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710396"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="66516-102">Adfs федерация сертификат с изтекъл срок</span><span class="sxs-lookup"><span data-stu-id="66516-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="66516-103">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="66516-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="66516-104">Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако модулът вече не е инсталиран).</span><span class="sxs-lookup"><span data-stu-id="66516-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="66516-105">За да направите това, отидете [на управление Azure AD с помощта на Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="66516-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="66516-106">Следвайте стъпките в "сценарий 1: AD FS маркер и подписване сертификат изтекъл" раздел ["Възникна проблем при достъп до сайта" грешка от AD FS при външен потребител влиза в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="66516-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="66516-107">Следвайте стъпките в [Актуализиране или поправяне на настройките на външен домейн в Microsoft, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="66516-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="66516-108">За да научите повече за подновяване на сертификати за обединяване, вижте [Подновяване федерация сертификати за Microsoft 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="66516-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
