---
title: Отстраняване на проблеми със сертификатите за SAML подписване
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692524"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Отстраняване на проблеми със сертификатите за SAML подписване

За да отстраните проблема със сертификат за подписване на SAML, изпълнете следните Препоръчителни стъпки:

1. Когато добавите корпоративна програма, която поддържа SSO, Azure ще генерира сертификат, наречен сертификат за подписване на [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Този сертификат има дата на изтичане на срока от 3 години. За да промените датата на изтичане на срока на вашия сертификат, вижте [Персонализиране на срока на валидност на сертификата на федерацията и прехвърлянето му към нов сертификат](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure ще използва този сертификат, за да подписва SAML жетони, поискани от приложението и да го изпрати към приложението за успешно SSO. За да завърши това, изтеглете сертификата от портала на Azure и го изпратете до производителя на приложението, за да завършите процеса на SSO.

След като този процес приключи, вашата кандидатура ще се довери на този сертификат и всички SAML маркери, подписани от този сертификат, ще бъдат приети от приложението.

3. Ако този сертификат изтече, създайте нов сертификат, актуализирайте го на доставчика на приложението и след това го направете активен в Azure. За повече информация вижте [подновяване на сертификат, който скоро ще изтече](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Ако сертификатът изтече, потребителят няма да бъде блокиран.

4. [Добавете имейл адрес за уведомленията](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , които трябва да бъдат получени, преди да изтече текущият сертификат.

> [!NOTE]
> Step-4 е незадължителен.

5. Промяна на опциите за подписване на приложението SAML сертификат и алгоритъм за подписване на сертификат. За повече информация вижте [Промяна на опциите за подписване на сертификат и алгоритъм за подписване](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

