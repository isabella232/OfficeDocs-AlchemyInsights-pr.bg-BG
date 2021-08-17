---
title: 726 Блокиране на препращането на имейли
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059621"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокиране или разблокиране на препращане на имейли

За да разрешите или забраните препращането на имейли за определена пощенска кутия, вижте [Конфигуриране на препращане на имейли](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

На ниво клиент управлението на външното препращане се извършва с помощта на правилата за изходяща спам. Можете да проверите правилата за изходящ филтър за [](https://protection.office.com/antispam) нежелана поща от центъра за защита и съответствие тук или с [помощта на командата Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Ако получавате следната грешка: **"550 5.7.520 Access е отказан,** Вашата организация не разрешава външно препращане" , уверете се, че правилата са конфигурирани да разрешават външно автоматично препращане.

**Забележка:** Препоръчва се външното автоматично препращане да бъде забранено във вашите правила за изходящи нежелана поща по подразбиране и да го разрешите само за потребителите, които се нуждаят от външно препращане, като създадете правила по избор за тези потребители. Можете да прочетете повече в [Конфигуриране на външно препращане на имейли в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).