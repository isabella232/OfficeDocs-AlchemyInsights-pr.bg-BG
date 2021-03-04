---
title: Отстраняване на неизправности при парола
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429348"
---
# <a name="troubleshoot-sspr"></a>Отстраняване на неизправности при парола

**Имам проблеми с настройването на нулирането на паролата**

- Ако сте администратор и търсите как да разрешите услугата за самостоятелно нулиране на паролата, вижте [урок разрешаване на парола](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), за да конфигурирате нулирането на паролата за вашата организация. Можете също да поискате да прегледате [изискванията за лицензиране](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Трябва да имате поне един лиценз, присвоен във вашата организация.
    - **Потребители в облака** – всеки Office 365 (O365) платен SKU или Azure ad Basic
    - **Облак и/или локални потребители** – Azure ad Premium P1 или P2, корпоративна мобилност + защита (EMS) или защитено продуктивно предприятие (спе)
- За допълнителни въпроси относно услугата за самостоятелно нулиране на паролата, прегледайте [нашите често задавани въпроси](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Получавам съобщение за грешка**

Прегледайте тази статия, за да намерите често срещани грешки и техните решения: [отстраняване на самостоятелно нулиране на паролата](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Имам проблем с правилата за нулиране на паролата**

- Ако политиката ви за нулиране на паролата не се държи според очакванията ви или ако имате въпроси относно правилата за нулиране на паролата, прегледайте тази статия: [правила и ограничения за парола в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Правилата за нулиране на паролата не се прилагат към администраторите. Microsoft налага строги правила за нулиране на пароли с две порти за всяка роля на администратор на Azure. Уверете се, че извършвате проверка с потребител, който не е администратор. За повече информация относно правилата за нулиране на администратора вижте тази статия: за [нулиране на правилата за администратора](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Не искам моите потребители да регистрират допълнителна информация за защита за нулиране на паролата**

Можете да попълвате предварително данни (имейл и телефонни атрибути) за вашите потребители, като използвате API, PowerShell или Azure AD Connect. За да научите как се чете:

- [Разполагане на нулиране на паролата, без да се изисква регистрация на потребителите](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Какви данни се използват чрез нулиране на паролата](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Искам моите потребители да регистрират своята допълнителна информация за защита за нулиране на паролата**

1. Помолете потребителите да регистрират своята информация за защита за услугата за самостоятелно нулиране на паролата, като ги насочат към [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. След като данните са попълнени за потребителя (от потребителя или от администратора), насочете потребителя си към [aka.MS/sspr](https://passwordreset.microsoftonline.com/) , така че потребителите да могат да бъдат оправомощени да нулират своите собствени пароли.
1. Ако потребителите все още имат проблеми, те са най-вероятно **външни** или **хеширани синхронизирани** потребители. Това означава, че е вероятно има проблем със услугата за нефиксирани на парола.