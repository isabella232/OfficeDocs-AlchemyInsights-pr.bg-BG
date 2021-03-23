---
title: Отстраняване на неизправности при протоколи OAuth 2,0 и OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034958"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Отстраняване на неизправности при протоколи OAuth 2,0 и OpenID Connect

За да отстраните проблеми с 2,0 и OpenID свързване на OAuth, изпълнете следните Препоръчителни стъпки:

Вижте следните статии, които са свързани с конфигурацията и отстраняването на неизправности OAuth 2,0 и протоколите за OpenID свързване:

- [Microsoft Identity Platform и OAuth 2,0 код за удостоверяване](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – тази статия описва как да програмирате директно спрямо **потока за даване на код (PKCE)** в приложението си, като използвате произволен език.
- [Платформата за самоличност на Microsoft и потокът на идентификационните данни за клиент на OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – тази статия описва как да програмирате директно към **потока идентификационни данни на клиента** във вашето приложение.
- [Платформа за самоличност на Microsoft и идентификационните данни за паролата на собственика на OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – тази статия описва как да програмирате директно спрямо **потока ROPC** в приложението.
    - Платформата за самоличност на Microsoft поддържа само ROPC за клиенти на Azure AD, но не и за лични акаунти. Това означава, че трябва да използвате конкретна крайна точка за **клиента https://login.microsoftonline.com/{TenantId_or_Name}) (** или крайна точка на **организациите** .
    - Лични акаунти, които са поканени на клиент на Azure AD, не могат да използват ROPC.
    - Акаунтите, които нямат пароли, не могат да влизат в ROPC. За този сценарий ви препоръчваме вместо това да използвате различен поток за вашето приложение.
    - Ако потребителите трябва да използват [многофакторно удостоверяване (МВнР)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , за да влязат в приложението, те ще бъдат блокирани.
    - ROPC не се поддържа за сценарии със [хибридната федерация за самоличност](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (НАПРИМЕР Azure ad и ADFS, използвани за удостоверяване на локални акаунти). Ако потребителите се пренасочват изцяло към локален доставчик на самоличност, Azure AD не е в състояние да изпробва потребителското име и паролата си за този доставчик на самоличност. [Транзитното удостоверяване](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) е подкрепено с ROPC.
    - Изключение за един сценарий на хибридна федерация за самоличност би било следното: правилата за откриване на Начало на **AllowCloudPasswordValidation** с набор от " **истина** ", ще позволят на ROPC Flow да работи за външни потребители, когато локалната парола е синхронизирана с облак. За повече информация вижте [Разрешаване на директно удостоверяване на ROPC на външни потребители за стари приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Платформата за самоличност на Microsoft и OAuth 2,0 от името на потока](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) -тази статия описва как да програмирате директно към **потока от името на (OBO)** в приложението.
- [Microsoft Identity Platform и протокол за свързване с OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – тази статия показва как да внедрите протокола за свързване с OpenID, независимо от езика, и описва как да изпращате и получавате HTTP съобщения, без да използвате никоя библиотека с отворен код на Microsoft.

**Маркери за достъп**

[Маркери за достъп до платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Научете как Вашият API може да провери и да използва претенциите в маркер на Access. Цялата документация в тази статия, освен в случаите, когато е посочена, се отнася само за маркери, издадени за API, които сте регистрирали. Той не се прилага за маркери, издадени за приложения, които са собственост на Microsoft, и тези маркери не могат да се използват за проверка как платформата за самоличност на Microsoft ще издаде маркери за създадения от вас API.

**Конфигуриране на приложение**

Настройки за [пренасочване (URL адрес на отговора) ограничения и ограничения](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Научете как да конфигурирате своя URI за пренасочване (URL адрес за отговор). URI за пренасочване или URL адресът на отговора е местоположението, където Сървърът за удостоверяване изпраща потребителя, след като приложението е успешно одобрено, и получи код за оторизация или маркер за достъп. Сървърът за удостоверяване изпраща кода или маркера към URI адреса за пренасочване; така че е важно да регистрирате правилното местоположение като част от процеса на регистрация на приложения.

**Обезпечаване на приложения**

[Урок: разработване и планиране на осигуряването за крайна точка на SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – тази статия описва как да създадете крайна точка на SCIM и да се интегрирате с услугата за осигуряване на пад.


