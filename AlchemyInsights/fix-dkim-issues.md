---
title: Отстраняване на проблеми с dKIM настройка
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717551"
---
# <a name="fix-dkim-setup-issues"></a>Отстраняване на проблеми с dKIM настройка

Ако имате проблеми, позволяващи DKIM за вашия домейн, използвайте следните стъпки:

- Повечето DKIM настройка проблеми са свързани с неправилни DNS записи. Проверете DKIM CNAME запис **(не** TXT запис) е форматиран правилно. За повече информация вижте тази [тема](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- След като създадете или актуализирате DKIM DNS записи в DNS хостинг услуга за вашия домейн (обикновено, вашия домейн регистратор), изчакайте DNS записите да се разпространяват.

- Ако не можете да създадете DKIM DNS записи в \<центъра\> за администриране, можете да замените CustomDomain с вашия потребителски `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`домейн (например contoso.com) и изпълнете тази команда в Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
