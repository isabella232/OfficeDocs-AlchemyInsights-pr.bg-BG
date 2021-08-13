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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919016"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Неупълномощена грешка в SharePoint

Ако получите грешката "(401) Неупълномощена" в SharePoint, тя може да е свързана с отстраняването на TLS 1.0/1.1. За допълнителна информация вж:

- [Подготовка за TLS 1,2 в Office 365 и Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Грешки при удостоверяване възникват, ако клиентът няма поддръжка на TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Актуализирайте, за да разрешите TLS 1.1 и TLS 1.2 като защитени протоколи по подразбиране в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ако потребителите са на Windows 7, проверете [TLS Cipher Suites в Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).