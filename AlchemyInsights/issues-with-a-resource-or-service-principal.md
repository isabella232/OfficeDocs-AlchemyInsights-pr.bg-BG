---
title: Проблеми с главен ресурс или услуга
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028065"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Проблеми с главен ресурс или услуга

1. Ако току-що започвате, основните обекти на приложението и услугата в [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) описват регистрацията на приложения, обектите на приложенията и на принципалите на услугата в Azure Active Directory: какви са те, как се използват и как са свързани помежду си. Примерен сценарий за много клиенти също се представя, за да се илюстрира релацията между обекта на приложението на приложението и съответните основни обекти на услугата.
2. Можете да научите повече за релацията между приложенията и принципалите на услугата, като прочетете приложенията и основните [обекти на услугата в Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Как да:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Използвайте портала, за да създадете основно приложение и услуга на Azure AD, които имат достъп до ресурсите, ви показва как да създадете ново приложение на Azure Active Directory (Azure AD) и принципал на услугата, които могат да се използват с контролата за достъп, базирана на роли.
4. С основния [API на услугата](https://docs.microsoft.com/graph/api/resources/serviceprincipal)можете програмно да управлявате екземпляри на приложения и да контролирате какво може да прави приложението в рамките на вашия клиент.
5. [servicePrincipal resource type lists](https://docs.microsoft.com/graph/api/resources/serviceprincipal) all properties and methods for the servicePrincipal resource type.
6. [Разликите в типа ресурси между Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) подчертават разликите между Azure AD Graph и ресурсите на Microsoft Graph. Показва ресурси, които имат различни имена или не са налични; Той също така подчертава ресурсите, налични в бета версията на Microsoft Graph, но не и във версията v1.0.

**Проблеми с потребителите на гости**

- [Бързо започване: Добавяне](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) на гости към вашия справочник в портала на Azure ви показва как да добавите нов потребител гост към вашия справочник на Azure AD чрез портала на Azure, да изпратите покана и да видите как изглежда процесът на осребряване на покана на потребителя.
- [Урок: Създаване на потребителски потоци в Azure Active Directory B2C ви](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) показва как да създадете някои препоръчителни потребителски потоци с помощта на портала на Azure. Ако търсите информация как да настроите поток от идентификационни данни за парола на собственик на ресурс (ROPC) във вашето приложение, вижте Конфигуриране на потока от идентификационни данни на собственика на ресурса в Azure AD B2C.
