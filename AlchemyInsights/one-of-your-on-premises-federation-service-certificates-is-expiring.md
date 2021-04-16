---
title: Един от вашите локални сертификати за услуги за федериране изтича
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810041"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Един от вашите локални сертификати за услуги за федериране изтича

За да разрешите този проблем, изпълнете следните стъпки:
  
- Инсталирайте модула на Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът все още не е инсталиран). За да направите това, отидете [на PowerShell на Azure Active Directory за Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Следвайте стъпките в раздела "Сценарий 1: Сертификатът за подписване на маркери на AD FS е изтекъл" на грешката "Възникна проблем с достъпа до сайта" от AD FS, когато федериран потребител влиза [в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Следвайте стъпките в Как да актуализирате или поправите настройките на федерирания домейн в [Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
За повече информация относно подновяването на сертификати за федериране вижте Подновяване на [сертификат за O365 и Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

