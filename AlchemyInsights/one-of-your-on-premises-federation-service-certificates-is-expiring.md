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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Изтича един от вашите локални сертификати за услуги на Федерацията

За да отстраните този проблем, изпълнете следните стъпки:
  
- Инсталирайте модула за Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът вече не е инсталиран). За да направите това, отидете в [Azure Active Directory PowerShell за Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Следване на стъпките в "сценарий 1: AD FS сертификатът за подписване с маркер с изтекъл срок" от ["Възникна проблем с достъпа до сайта" от AD FS, когато един външен потребител влезе в Microsoft 365, Azure или в съзвучие](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Следвайте стъпките в [как да актуализирате или поправите настройките на външен домейн в Microsoft 365, Azure или за настройка](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
За повече информация относно подновяването на сертификатите на Федерацията вижте [подновяване на сертификат за O365 и AZURE ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

