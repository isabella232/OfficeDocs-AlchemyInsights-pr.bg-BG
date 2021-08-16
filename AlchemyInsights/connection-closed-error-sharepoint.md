---
title: Базовата връзка е затворена грешка в SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044401"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Грешка "Базовата връзка е затворена" в SharePoint

Ако получавате грешката "Базовата връзка е затворена" в SharePoint, тя може да е свързана с отменението на TLS 1.0/1.1. За повече информация вижте следните статии:

- [Подготовка за TLS 1,2 в Office 365 и Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Грешки при удостоверяване възникват, ако клиентът няма поддръжка на TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Актуализирайте, за да разрешите TLS 1.1 и TLS 1.2 като защитени протоколи по подразбиране в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ако потребителите са на Windows 7, проверете [TLS Cipher Suites в Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).