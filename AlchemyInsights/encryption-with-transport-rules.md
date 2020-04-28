---
title: Шифроване с транспортни правила
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915019"
---
# <a name="encryption-with-transport-rules"></a>Шифроване с транспортни правила

В [център за администриране на Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), можете да използвате възможностите за шифроване на съобщения в Office (OME) в правилата за пощенския поток, за да задействате шифроването на съобщения. Изберете опцията **Прилагане на шифроване на съобщения в Office 365 и защита на правата за достъп** към условието за правило за транспорт.

- За повече информация вж. [Дефиниране на правилото за пощенския поток за шифроване](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- В PowerShell използвайте кратката команда [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и настройте параметъра *ApplyOME* на $true.
