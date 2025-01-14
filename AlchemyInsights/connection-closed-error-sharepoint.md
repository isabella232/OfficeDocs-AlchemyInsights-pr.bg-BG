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
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317685"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Грешка "Базовата връзка е затворена" в SharePoint

Ако получавате грешката "Базовата връзка е затворена" в SharePoint, тя може да е свързана с отстраняването на TLS 1.0/1.1. За повече информация вижте следните статии:

- [Подготовка за TLS 1,2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Грешки при удостоверяване възникват, ако клиентът няма поддръжка на TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Актуализирайте, за да разрешите TLS 1.1 и TLS 1.2 като защитени протоколи по подразбиране в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ако потребителите са на Windows 7, уверете се, че [проверяват TLS Cipher Suites в Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).