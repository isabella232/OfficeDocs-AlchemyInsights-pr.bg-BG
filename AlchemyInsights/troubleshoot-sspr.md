---
title: Отстраняване на неизправности с SSPR
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038947"
---
# <a name="troubleshoot-sspr"></a>Отстраняване на неизправности с SSPR

**Имам проблеми с конфигурирането на нулиране на паролата**

- Ако сте администратор и търсите как да разрешите самостоятелно нулиране на паролата, вижте Ръководство за разрешаване [на SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), за да конфигурирате нулирането на паролата за вашата организация. Може също да поискате да прегледате изискванията [за лицензиране](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Трябва да имате поне един лиценз, присвоен във вашата организация.
    - **Само за потребители в** облака – Office 365 (O365) платен SKU или Azure AD Basic
    - **Потребители в облака и/или** локални потребители – Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)
- За допълнителни въпроси относно самостоятелното нулиране на пароли прегледайте [нашите ЧЗВ.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Получавам съобщение за грешка**

Прегледайте тази статия, за да намерите често срещани грешки и техните решения: Отстраняване на неизправности [при самостоятелно нулиране на пароли](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Имам проблем с правилата за нулиране на паролата**

- Ако правилата ви за нулиране на паролата не се държат според очакванията или ако имате въпроси относно правилата за нулиране на паролата, прегледайте тази статия: Правила за [пароли и ограничения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Правилата за нулиране на пароли не важат за администраторите. Microsoft налага силни правила за нулиране на две портове по подразбиране за всяка роля на администратор на Azure. Уверете се, че тествате с потребител, който не е администратор. За повече информация относно правилата за нулиране на администратор вижте тази статия: Разлики в правилата [за нулиране на администратор.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Не искам моите потребители да регистрират допълнителна информация за защита за нулиране на паролата**

Можете да попълвате предварително данни (атрибути за имейл и телефон) за вашите потребители чрез API, PowerShell или Azure AD Свързване. За да научите как да четете:

- [Разполагане на нулиране на паролата, без да се изисква от потребителите да се регистрират](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Какви данни се използват при нулиране на паролата](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Искам моите потребители да регистрират допълнителната си информация за защита за нулиране на паролата**

1. За да могат вашите потребители да регистрират своята информация за защита за самостоятелно нулиране на паролата, като ги [напът aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. След като данните са попълнени за потребителя (от потребителя или от администратора), насоте потребителя [към aka.ms/sspr,](https://passwordreset.microsoftonline.com/) така че потребителите ви да могат да бъдат упълномощени да нулират собствените си пароли.
1. Ако потребителите все още изпитват проблеми, те най-вероятно **са федерирани** или потребители, които имат **синтаксис на пароли.** Това означава, че вероятно има проблем с услугата за обратно записване на пароли.