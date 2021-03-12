---
title: Проблеми с ресурс или услуга принципал
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713352"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Проблеми с ресурс или услуга принципал

1. Ако току-що сте първи стъпки, [основните обекти за приложения и услуги в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) описват регистрацията на приложения, обектите на приложението и основните услуги в Azure Active Directory: Какво представляват, как се използват и как те се отнасят един към друг. Примерен сценарий за мулти-клиент се представя и за илюстриране на релацията между обекти на приложения на приложението и съответстващи основни обекти за услуги.
2. Можете да научите повече за релацията между приложенията и основните услуги, като прочетете [приложения и основни обекти за услуги в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Как да: използвайте портала, за да създадете приложение за приложения и услуги на AZURE ad, което има достъп до ресурсите](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) ви показва как да създадете ново приложение за Azure Active Directory (Azure ad), което може да се използва с базираното на роли управление на достъпа.
4. Чрез [основния програмен интерфейс на услугата](https://docs.microsoft.com/graph/api/resources/serviceprincipal)можете да управлявате по програмен път екземплярите на приложения и да управлявате какво може да прави приложението във вашия клиент.
5. [тип ресурс на servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) изброява всички свойства и методи за типа ресурс на servicePrincipal.
6. [Различията между типовете ресурси между AZURE ad Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) осветяват разликите между Azure ad Graph и ресурси на Microsoft Graph. Показва ресурси, които имат различни имена или не са налични; то също така осветява наличните ресурси в бета-версията на Microsoft Graph, но не и във версията v 1.0.

**Проблеми с гост потребители**

- Бърз [Старт: Добавяне на гости към вашия указател в портала на Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) ви показва как да добавите нов гост към директорията на Azure ad чрез портала на Azure, да изпратите покана и да видите как изглежда процесът за изкупуване на поканата на потребителя за гост.
- [Урок: създаване на потребителски потоци в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) ви показва как да създадете някои Препоръчителни потребителски потоци с помощта на портала на Azure. Ако търсите информация как да настроите източник на данни за парола на собственик на ресурс (ROPC) в своето приложение, вижте конфигуриране на данни за парола на собственика на ресурса в Azure AD B2C.
