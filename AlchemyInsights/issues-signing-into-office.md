---
title: Проблеми с влизането в Microsoft 365 приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744621"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Проблеми с влизането в Приложения на Microsoft 365

Забележка: Ако използвате по-стара версия на Windows (например Windows 7 SP1, Windows Server 2008 R2), използвайте лесната корекция, за да [разрешите](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) TLS 1.2 по подразбиране. За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows.

За да коригирате проблеми с влизането Microsoft 365 приложения, изпробвайте следните опции на засегнатия компютър:  

- За Windows вижте [Препоръки за разрешаване на често срещани проблеми при влизане](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- За Mac вижте [Не може да влезете в приложение Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Съвет** На Windows компютри можем да диагностицираме и автоматично да коригираме няколко често срещани Office за влизане. Изтеглете и стартирайте **[microsoft Помощник за поддръжка и възстановяване,](https://aka.ms/SaRA-OfficeSignInScenario)** за да използвате нашия автоматизиран инструмент.

**Забележка:** Забраняването на модерното удостоверяване (ADAL) или управлението на уеб акаунти (WAM) за отстраняване на проблеми с влизането или активирането **не се препоръчва.** Ако възникнат грешки при свързване към Microsoft 365 с Office 2013, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) уверете се, че разрешавате модерно удостоверяване за Office клиент.

За конкретни действия за отстраняване на неизправности вижте:

[Проблеми с връзката при влизане след актуализация до Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Не можете да влезете в своя организационно акаунт, като Office 365, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Как да отстранявате неизправности с приложения, които не са браузъри, които не могат да впишат в Office 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Многократно подкана за идентификационни данни в Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)