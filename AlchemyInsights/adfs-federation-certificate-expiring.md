---
title: ADFS федерация сертификата изтича
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
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499880"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a781e-102">ADFS федерация сертификата изтича</span><span class="sxs-lookup"><span data-stu-id="a781e-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a781e-103">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="a781e-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a781e-104">Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако вече не е инсталиран модул).</span><span class="sxs-lookup"><span data-stu-id="a781e-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a781e-105">За да направите това, отидете в [управление лазурно АД чрез Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="a781e-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="a781e-106">Следвайте стъпките в "сценарий 1: AD FS маркер за подписване сертификат с изтекъл срок" раздел на ["Възникнал е проблем при достъпа до сайта" грешка от AD FS когато външно потребител влезе в Office 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a781e-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="a781e-107">Следвайте стъпките в [как да актуализирате или да поправите настройките на външен домейн в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="a781e-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="a781e-108">За да научите повече за подновяване федерация сертификати, вижте [поднови федерация сертификати за Office 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a781e-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
