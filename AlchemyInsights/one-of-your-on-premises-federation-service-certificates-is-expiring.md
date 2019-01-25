---
title: Един от вашите сертификати за услуга на локалния федерация е expiring
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458060"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Един от вашите сертификати за услуга на локалния федерация е expiring

За да разрешите този проблем, изпълнете следните стъпки:
  
- Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако вече не е инсталиран модул). За да направите това, отидете на [Azure Active Directory PowerShell за графика](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Следвайте стъпките в "сценарий 1: AD FS маркер за подписване сертификат с изтекъл срок" раздел на ["Възникнал е проблем при достъпа до сайта" грешка от AD FS когато външно потребител влезе в Office 365, Azure или Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Следвайте стъпките в т[как да актуализирате или да поправите настройките на външен домейн в Office 365, Azure или Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
За повече информация относно подновяване федерация сертификати вижте [подновяване на сертификат за O365 и лазурно АД](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

