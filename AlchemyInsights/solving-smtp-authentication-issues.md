---
title: Разрешаване на SMTP удостоверяване и отстраняване на неизправности
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077640"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Разрешаване на SMTP удостоверяване и отстраняване на неизправности

Ако искате да разрешите SMTP удостоверяване за пощенска кутия или получавате грешка "Клиентът не е удостоверен", "Неуспешно удостоверяване" или "SmtpClientAuthentication" с код 5.7.57 или 5.7.3 или 5.7.139, когато се опитате да препредавате имейл чрез удостоверяване на устройство или приложение с Microsoft 365, изпълнете тези три действия, за да разрешите проблема:

1. [Забранете настройките за защита на Azure по подразбиране,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) като превключвате **разрешаването на защита по подразбиране** на **Не**.

    a. Влезте в портала на Azure като администратор на защитата, администратор на условен достъп или глобален администратор.<BR/>
    б. Отидете до Azure Active Directory > **свойства**.<BR/>
    в. Изберете **Управление на настройките по подразбиране за защита**.<BR/>
    г. Задайте **Разрешаване на настройките по подразбиране за защита** на **Не**.<BR/>
    д. Изберете **Записване**.

2. [Разрешаване на изпращането на SMTP на](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) клиента в лицензираната пощенска кутия.

    a. От Център за администриране на Microsoft 365 отидете на **Активни потребители** и изберете потребителя.<BR/>
    б. Отидете в раздела Поща и под Приложения **за имейл изберете** Управление на имейл **приложения**.<BR/>
    г. Уверете се, **че удостоверен SMTP** е отметнато (разрешено).<BR/>
    д. Изберете **Запиши промените**.<BR/>

3. [Забраняване на многофакторното удостоверяване (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) в лицензираната пощенска кутия.

    a. Отидете на Център за администриране на Microsoft 365 и в менюто за навигация отляво изберете **Потребители**  >  **Активни потребители**.<BR/>
    б. Изберете **Многофакторно удостоверяване**.<BR/>
    в. Изберете потребителя и **забранете многофакторното удостоверяване**.<BR/>
