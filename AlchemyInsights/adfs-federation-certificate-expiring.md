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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952958"
---
# <a name="adfs-federation-certificate-expiring"></a>Изтичане на срока на сертификата за федериране на ADFS

За да разрешите този проблем, изпълнете следните стъпки:
  
1. Инсталирайте Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът още не е инсталиран). За да направите това, отидете на [Управление на Azure AD с помощта на Windows PowerShell](https://aka.ms/aadposh).

2. Следвайте стъпките в раздела "Сценарий 1: Сертификатът за подписване на маркери на AD FS е изтекъл" на грешката "Възникна проблем с достъпа до сайта" от AD FS, когато федериран потребител влиза [в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Следвайте стъпките в [Актуализиране или поправяне на настройките на федерирания домейн в Microsoft, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    За да научите повече за подновяването на сертификати за федериране, вижте Подновяване на [сертификати за федериране за Microsoft 365 и Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
