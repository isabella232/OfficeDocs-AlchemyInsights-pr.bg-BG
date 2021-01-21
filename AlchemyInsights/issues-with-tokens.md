---
title: Проблеми с маркери
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916693"
---
# <a name="issues-with-tokens"></a>Проблеми с маркери

За да управлявате проблемите, свързани с маркери, можете да изпълните следните стъпки:

1. Можете да укажете живота на маркер на Access, ИД или SAML, издаден от платформата за самоличност на Microsoft. Можете да зададете маркери за цял живот за всички приложения във вашата организация, за приложение за много клиенти (мултиорганизация) или за определен принципал на услуга във вашата организация. За повече информация вижте [конфигурируеми животи с маркери в Microsoft Identity Platform (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Маркерите на Access разрешават на клиентите безопасно да се обаждат на защитени уеб API и се използват от уеб API за извършване на удостоверяване и упълномощаване. Както по спецификацията за OAuth, маркерите на Access са непрозрачни низове без зададен формат – някои доставчици на самоличност (Врл) използват GUID, други използват шифровани петна. Платформата за самоличност на Microsoft използва различни формати за маркери на Access в зависимост от конфигурацията на API, който приема маркера. За да научите как Вашият API може да провери и да използва претенциите в маркер на Access, вижте [маркери за достъп до платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Библиотеката за удостоверяване на Microsoft (MSAL) поддържа няколко потока на удостоверяване за използване в различни сценарии за приложения. За повече информация вижте [потоци на удостоверяване](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Помощта за разрешаване на OAuth 2,0 може да се използва в приложения, които са инсталирани на устройство, за да получат достъп до защитени ресурси, като например Web API. С помощта на платформата за самоличност на Microsoft за изпълнение на OAuth 2,0 можете да добавите влизане и достъп до API към вашите мобилни и настолни приложения. Вижте [Microsoft Identity Platform и OAuth 2,0 за разрешаване на код](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) за програмата за как да програмирате директно спрямо Протокола във вашето приложение, като използвате произволен език.
5. OpenID Connect (OIDC) е протокол за удостоверяване, изграден върху OAuth 2,0, който можете да използвате за защитено влизане на потребител в приложение. Когато използвате приложението за крайна точка на платформата за самоличност на Microsoft с OpenID Connect, можете да добавите влизане и достъп до API към приложенията си. [Платформата за самоличност на Microsoft и Протоколът за OpenID свързване](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) показва как да направите това независимо от езика и как да изпращате и получавате HTTP съобщения, без да използвате никоя библиотека с отворен код на Microsoft.
    - Крайна точка UserInfo е част от OIDC стандарт, предназначени за връщане на рекламации за потребителя, който е удостоверен. За повече информация вижте [крайна точка за Microsoft Identity Platform UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Обаждането на уеб API в уеб приложение чрез AZURE ad и OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) пример показва как да създадете MVC уеб приложение, което използва Azure ad за влизане чрез протокола за OpenID Connect, а след това да се обадите на уеб API под самоличността на потребителя, който използва маркери, получени чрез OAuth 2,0. Тази извадка използва приложението OpenID Connect ASP .net OWIN и ADAL .net.
6. [Конфигуриране на приложение за изложите уеб API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – в този бърз старт можете да регистрирате уеб API с платформата Microsoft Identity и да я излагате на клиентски приложения, като добавите примерен обхват. Чрез регистрирането на вашия уеб API и изпробването му през обхвати можете да предоставяте достъп на разрешения до ресурсите си за оторизирани потребители и клиентски приложения, които осъществяват достъп до вашия API.
7. В Azure Active Directory B2C (Azure AD B2C), Flow идентификационни данни за парола на собственик на ресурс (ROPC) е OAuth стандартния поток за удостоверяване. В този поток приложение, което е известно като доверяващо се страна, обменя валидни идентификационни данни за жетони. Идентификационните данни включват потребителски ИД и парола. Върнатите маркери са ИД маркер, маркер за достъп и маркер за обновяване. За повече информация вижте [Настройване на удостоверяване на парола за собственик на ресурс в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

