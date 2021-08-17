---
title: Шифроване с транспортни правила
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
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079439"
---
# <a name="encryption-with-transport-rules"></a>Шифроване с транспортни правила

В [център за администриране на Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), можете да използвате възможностите за шифроване на съобщения в Office (OME) в правилата за пощенския поток, за да задействате шифроването на съобщения. Изберете опцията **Прилагане на шифроване на съобщения в Office 365 и защита на правата за достъп** към условието за правило за транспорт.

- За повече информация вж. [Дефиниране на правилото за пощенския поток за шифроване](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- В PowerShell използвайте кратката команда [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и настройте параметъра *ApplyOME* на $true.
