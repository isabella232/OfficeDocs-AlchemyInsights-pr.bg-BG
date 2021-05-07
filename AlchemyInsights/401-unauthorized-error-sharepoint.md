---
title: 401 Неупълномощена грешка в SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233487"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Неупълномощена грешка в SharePoint

Ако получите грешката "(401) Неупълномощена" в SharePoint, тя може да е свързана с отстраняването на TLS 1.0/1.1. За допълнителна информация вж:

[Подготовка за TLS 1,2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Грешки при удостоверяване възникват, ако клиентът няма поддръжка на TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Ако потребителите са на Windows 7, проверете [TLS Cipher Suites в Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).