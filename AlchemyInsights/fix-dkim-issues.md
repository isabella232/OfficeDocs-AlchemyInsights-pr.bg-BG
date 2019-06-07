---
title: Прикрепвам проблеми с инсталирането на DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764845"
---
# <a name="fix-dkim-setup-issues"></a>Прикрепвам проблеми с инсталирането на DKIM

Ако имате въпроси, позволяващи DKIM за потребителски домейна, използвайте следните стъпки:

- Повечето DKIM настройка проблеми са свързани с неправилен DNS записи. Проверете DKIM CNAME запис (**не** TXT запис) е форматиран правилно. За повече информация вижте тази [тема](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- След като създадете или актуализирате вашите DKIM DNS записи в услугата за DNS хостинг за вашия домейн (обикновено вашия регистратор на домейн), изчакайте за DNS, записите да пропагандира.

- Ако не може да създадете DKIM DNS записи в центъра на администратор, можете да замените \<CustomDomain\> с вашия собствен домейн (например contoso.com) и стартирате тази команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
