---
title: Блокиране или разблокиране на външно автоматично препращане на имейли
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315863"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Блокиране или разблокиране на вечно автоматично препращане на имейли

За да разрешите или забраните препращането на имейл за определена пощенска кутия, вижте [Конфигуриране на препращане на имейли](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Администраторите могат да контролират външното препращане за организацията с помощта [на правила за изходяща спам.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Можете да управлявате правилата за изходяща спам в Microsoft 365 Defender портала на или с <https://security.microsoft.com/antispam> [помощта на кратката команда Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) в Exchange Online PowerShell.

Ако получите следната грешка: **"550 5.7.520 Access е отказан,** вашата организация не позволява външно препращане", уверете се, че правилата са конфигурирани да разрешават външни автоматично препратени съобщения.

**Забележка:** Препоръчваме стойността по подразбиране Автоматично  **– система,** управлявана за настройката на правилата за автоматично препращане във вашите правила за изходяща нежелана поща по подразбиране (автоматичното външно препращане е блокирано; вътрешното автоматично препращане все още работи). Трябва да създадете правила за потребителски изходящ филтър за нежелана поща и да използвате стойността **Включено –** препращането е разрешено само за потребители, които се нуждаят от външно автоматично препращане на имейли. За повече информация вижте Конфигуриране [на външно препращане на имейли в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
