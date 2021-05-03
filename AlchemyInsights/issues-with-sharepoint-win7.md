---
title: Проблеми с SharePoint на Windows 7 машини
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124815"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Проблеми с SharePoint на Windows 7 машини

Ако получите грешки на Windows 7 машини, докато работите на SharePoint или OneDrive, те може да са свързани с отстраняването на TLS 1.0/1.1. За повече информация вижте:

- [Подготовка за TLS 1,2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 трябва да имат разрешен TLS1.2. За повече информация вижте Грешки [при удостоверяване възникват, когато клиентът няма поддръжка на TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Инсталирайте KB3140245 и създайте стойността в системния регистър. За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) като защитени протоколи по подразбиране в WinHTTP в Windows

- Windows 7 SP1/Windows 8 трябва да гарантират, че са инсталирани най-новите пакети за шифроване на TLS. За повече информация вижте [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


