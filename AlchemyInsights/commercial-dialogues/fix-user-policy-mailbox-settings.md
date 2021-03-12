---
title: Коригиране на настройките на потребителските правила/пощенските кутии
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743861"
---
# <a name="fix-user-policymailbox-settings"></a>Коригиране на настройките на потребителските правила/пощенските кутии

Настройките за нежелана поща в пощенската кутия са засегнали това съобщение. За да прегледате настройките, направете следното:

1. Стартиране на обвивката за управление на Exchange. За повече информация вижте [Отваряне на обвивката за управление на Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Изпълнете тази команда (като използвате имейл адреса на потребителя):  **get-mailboxjunkmailconfiguration-самоличност "User@domain.com"**
3. Проверете дали имейл адресът на подателя е част от **TrustedSendersAndDomains** , или **BlockedSendersAndDomains**. Ако имейл адресът е в един от списъците, може да се наложи да го премахнете. За да научите повече, вижте [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
