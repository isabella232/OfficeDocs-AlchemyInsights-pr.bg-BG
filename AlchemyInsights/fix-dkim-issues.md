---
title: Коригиране на проблеми с настройката на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945920"
---
# <a name="fix-dkim-setup-issues"></a>Коригиране на проблеми с настройката на DKIM

Ако имате проблеми с разрешаването на DKIM за вашия домейн по избор, използвайте следните стъпки:

- Повечето проблеми с настройката на DKIM са свързани с неправилни DNS записи. Проверете дали DKIM CNAME записът **(а** не TXT запис) е форматиран правилно. За повече информация вижте тази [тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- След като създадете или актуализирате своите DKIM DNS записи в DNS хостинг услугата за вашия домейн (обикновено регистратор на домейни), изчакайте DNS записите да се разпространяват.

- Ако не можете да създадете DKIM DNS записите в центъра за администриране, можете да заместите с вашия домейн по избор (например contoso.com) и да изпълните тази команда \<CustomDomain\> [в Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
