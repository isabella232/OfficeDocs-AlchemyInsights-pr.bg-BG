---
title: Безшевни проблеми при влизане на SSO потребители
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935080"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Безшевни проблеми при влизане на SSO потребители

След като потребителят е удостоверен, браузърът ще кешира идентификационните данни на потребителя, така че в един и същ браузър приложението автоматично ще влиза със същия акаунт. Това може да е трудно за друг потребител или отделен потребител да се регистрира в няколко акаунта на едно устройство. За да решите това: 1. Опитайте да влезете в друг браузър. 2. Изчистете кеша и/или бисквитките на браузъра и опитайте да влезете отново.

Ако все още имате проблеми с влизането, ви препоръчваме следното, за да диагностицирате и автоматизирате стъпките за разрешаване:

1. Инсталирайте [разширението за защитен браузър "моите приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) ", за да помогнете на Azure Active Directory (Azure ad) да осигури по-добра диагноза и резолюции при използването на тестовата среда в портала на Azure.
2. Възпроизведете грешката с помощта на тестовата среда в страницата за конфигуриране на приложението в портала на Azure. За да научите повече, вижте [отстраняване на грешки при SAML-базирани приложения за еднократна идентификация](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Ако използвате функцията за тестване в портала на Azure с разширението за защитен браузър "моите приложения", можете да **пропуснете стъпка 4**.
4. За да отворите страницата за конфигуриране на еднократна идентификация на SAML:
    - Отворете [портала на Azure](https://portal.azure.com/) и влезте като **глобален администратор** или **съадминистратор**.
    - Отворете **разширението на Azure Active Directory** , като изберете **всички услуги** в горния край на главното навигационното меню в ляво.
    - Въведете "Azure Active Directory" в полето за търсене на филтър и изберете елемента на **Azure Active Directory** .
    - Изберете **корпоративни приложения** от менюто за навигация в Azure Active Directory.
    - Изберете **всички приложения** , за да видите списък на всички свои приложения. Ако не виждате приложението, което искате да се показва тук, използвайте контролата за **филтър** в горния край на списъка с **всички приложения** и задайте опцията **Покажи** за **всички приложения**.
    - Изберете приложението, което искате да конфигурирате за еднократна идентификация.
    - След като приложението се зареди, изберете **еднократна идентификация** от лявото меню за навигация в приложението.
    - Изберете **SAML, базиран на SSO**.
5. Въз основа на грешката, за да научите повече за препоръчваните стъпки за следване, вижте [проблеми при влизане в конфигурирани приложения за еднократна идентификация, базирани на SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. За да отстраните други потребителски проблеми при влизане, вижте следните насоки:
    - [SAML протокол за единична Sign-On](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Как да: отстраняване на грешки при влизане чрез отчетите за Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Подкана за неочаквано съгласие](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Грешка при съгласие на потребителя](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Проблеми при влизане от моите приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Грешка на страницата за влизане в приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Проблем при влизане в приложение на Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
