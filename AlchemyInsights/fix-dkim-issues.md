---
title: Отстраняване на проблеми при настройване на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506763"
---
# <a name="fix-dkim-setup-issues"></a>Отстраняване на проблеми при настройване на DKIM

Ако имате проблеми с DKIM за вашия домейн, използвайте следните стъпки:

- Повечето DKIM настройка проблеми са свързани с неправилни DNS записи. Проверете DKIM CNAME запис **(не** TXT запис) е форматиран правилно. За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- След като създадете или актуализирате DKIM DNS записи в DNS хостинг услугата за вашия домейн (обикновено, вашия регистратор на домейни), изчакайте DNS записи да се разпространяват.

- Ако не можете да създадете DKIM DNS записи в центъра за администриране, можете да \<CustomDomain\> замените с вашия потребителски домейн (например contoso.com) и да изпълните тази команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
