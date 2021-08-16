---
title: Коригиране на настройките за потребителски правила/пощенски кутии
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034707"
---
# <a name="fix-user-policymailbox-settings"></a>Коригиране на настройките за потребителски правила/пощенски кутии

Настройките за нежелана поща в пощенската кутия са засегнати от това съобщение. За да прегледате настройките, направете следното:

1. Стартирайте Exchange за управление. За повече информация вижте Отваряне [на обвивката Exchange за управление.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Изпълнете тази команда (като използвате имейл адреса на потребителя):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Проверете дали имейл адресът на подателя е част от **TrustedSendersAndDomains** или **BlockedSendersAndDomains**. Ако имейл адресът е в един от списъците, може да се наложи да го премахнете. За да научите повече, вижте [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
