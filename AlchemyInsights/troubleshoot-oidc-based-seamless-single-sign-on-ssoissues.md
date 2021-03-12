---
title: Отстраняване на неизправности при проблеми с еднократната идентификация, базирани на OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743188"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Отстраняване на неизправности при проблеми с еднократната идентификация, базирани на OIDC

- За да научите как да добавите приложение, базирано на OIDC, към вашия клиент на Azure, вижте бърз [Старт: Настройване на еднократна идентификация на OIDC (SSO) за приложение в Azure Active Directory (AZURE ad) клиент](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- За повече информация за приложенията, които използват стандарта за OpenID Connect за реализиране на еднократна идентификация, вижте [разбиране на OIDC, базирано на еднократна идентификация](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- За информация в случай че изберете да напишете кода си, като директно изпращате и обработвате HTTP заявки или използвате библиотека с отворен код на трети страни, вместо да използвате една от нашите библиотеки с отворен код, вижте [OAuth 2,0 и протоколи за свързване с OpenID на платформата Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Протоколи**

1. [Платформата за самоличност на Microsoft и неявните потоци за даване](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – дефинираната характеристика на неявните безвъзмездни средства е, че МАРКЕРИ (ИД маркери или маркери за достъп) се връщат директно от крайна точка на/Authorize вместо крайна точка на/token. Това често се използва като част от потока на кодовете за удостоверяване в това, което се нарича **"хибриден поток" – извличане на идентификационния маркер в искането за/Authorize заедно с код за удостоверяване**. Тази статия описва как да програмирате директно спрямо Протокола във вашето приложение, за да поискате маркери от Azure AD.
2. [Microsoft Identity Platform и OAuth 2,0 код за оторизиране на оторизация](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – OAuth 2,0 упълномощаване на кодове за даване могат да се използват в приложения, които са инсталирани на устройство, за да получат достъп до защитени ресурси, като например Web API. С помощта на платформата за самоличност на Microsoft за изпълнение на OAuth 2,0 можете да **добавите влизане и достъп до API към вашите мобилни и настолни приложения**. Тази статия описва как да програмирате директно спрямо Протокола във вашето приложение, като използвате произволен език.
3. [Платформа за самоличност на Microsoft и протокол за свързване с OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – когато използвате Microsoft Identity Platform за изпълнение на OpenID Connect, можете да добавите влизане и достъп до API за приложенията си. Тази статия показва как да направите това независимо от езика и как да **изпращате и получавате HTTP съобщения, без да използвате каквито и да е библиотеки с отворен код на Microsoft**.
4. [Платформата за самоличност на Microsoft и потокът на идентификационните данни за клиент на OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – можете да използвате идентификационните данни за клиент на OAuth 2,0, указани в RFC 6749, понякога наричан **двустепенен OAuth**, за да имате достъп до уеб хоствани ресурси с помощта на самоличността на приложение. Този тип субсидия обикновено се използва за взаимодействия между сървърите и сървърите, които трябва да се изпълняват във фона, без незабавно взаимодействие с потребител. Тези типове приложения често биват наричани **демон** или **акаунт за услуги**. Тази статия описва как да програмирате директно спрямо Протокола във вашето приложение.
