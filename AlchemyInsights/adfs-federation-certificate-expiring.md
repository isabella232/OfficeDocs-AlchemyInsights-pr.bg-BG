---
title: Изтича сертификат за ADFS на Федерацията
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686703"
---
# <a name="adfs-federation-certificate-expiring"></a>Изтича сертификат за ADFS на Федерацията

За да отстраните този проблем, изпълнете следните стъпки:
  
1. Инсталирайте модула за Microsoft Azure Active Directory за Windows PowerShell на компютъра (ако модулът вече не е инсталиран). За да направите това, отидете на [управление на AZURE ad с помощта на Windows PowerShell](https://aka.ms/aadposh).

2. Следване на стъпките в "сценарий 1: AD FS сертификатът за подписване с маркер с изтекъл срок" от ["Възникна проблем с достъпа до сайта" от AD FS, когато един външен потребител влезе в Microsoft 365, Azure или в съзвучие](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Следвайте стъпките в [актуализиране или поправяне на настройките на външен домейн в Microsoft, Azure или в настройка](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    За да научите повече за подновяването на сертификатите на федерацията, вижте [подновяване на сертификатите на Федерацията за Microsoft 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
