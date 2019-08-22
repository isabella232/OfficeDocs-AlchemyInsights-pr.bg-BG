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
# <a name="adfs-federation-certificate-expiring"></a>ADFS федерация сертификата изтича

За да разрешите този проблем, изпълнете следните стъпки:
  
1. Инсталирайте Microsoft Azure Active Directory модул за Windows PowerShell на компютъра (ако вече не е инсталиран модул). За да направите това, отидете в [управление лазурно АД чрез Windows PowerShell](https://aka.ms/aadposh).

2. Следвайте стъпките в "сценарий 1: AD FS маркер за подписване сертификат с изтекъл срок" раздел на ["Възникнал е проблем при достъпа до сайта" грешка от AD FS когато външно потребител влезе в Office 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Следвайте стъпките в [как да актуализирате или да поправите настройките на външен домейн в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    За да научите повече за подновяване федерация сертификати, вижте [поднови федерация сертификати за Office 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
