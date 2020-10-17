---
title: 726, който блокира препращането на имейли
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473090"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокиране или разблокиране на препращане на имейли

За да разрешите или забраните препращането на имейли за конкретна пощенска кутия, вижте [Конфигуриране на препращане на имейл](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

На ниво клиент контролата за външно препращане се осъществява чрез правилата за изходящи спам. Можете да проверите правилата за изходящ филтър за нежелана поща от центъра за защита и съответствие [тук] ( https://protection.office.com/antispam) или с помощта на [командата get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Ако получавате следното съобщение за грешка: **"550 5.7.520 отказан достъп, вашата организация не разрешава външно препращане"**, моля, уверете се, че правилата са конфигурирани за разрешаване на външни автоматични препращания.

**Забележка:** Препоръчително е да запазите неактивираните външни автоматично препращане на правилата за изходящите филтри за нежелана поща и да я разрешите само за потребителите, които се нуждаят от външно препращане, като създадат правила по избор за тези потребители. Можете да прочетете повече за [конфигурирането на външно препращане на имейли в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).