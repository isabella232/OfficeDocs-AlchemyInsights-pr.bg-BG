---
title: API Permissions and Consent Process
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404225"
---
# <a name="api-permissions-and-consent-process"></a>API Permissions and Consent Process

За да може вашето приложение да има достъп до данни в Microsoft Graph, потребителят или администраторът трябва да му даде правилните разрешения чрез процес на съгласие. [Препратките към разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) изброяват разрешенията, свързани с всеки основен набор от API на Microsoft Graph. Той също така предоставя указания как да използвате разрешенията.

**Настройване или актуализиране на главен директор на услугата**

- [Създаване на принципна услуга](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – тази статия ви показва как да създадете нов обект на услугаПринципално.
- [Създаване на приложение azure AD & на](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) услугата в портала – Тази статия ви показва как да създадете ново приложение на Azure Active Directory (Azure AD) и принципал на услугата, които могат да се използват с контролата за достъп, базирана на роли.
- [Приложения &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) на услуги в Azure AD – тази статия описва регистрацията на приложения, обектите на приложенията и директорите на услуги в Azure Active Directory: какви са те, как се използват и как те са свързани помежду си.

**Добавяне или актуализиране на регистрацията на приложения и предоставяне на съгласие от администратор**

- [Създаване на регистрация на приложение](https://docs.microsoft.com/graph/api/application-post-applications) – тази статия ви показва как да създадете нов обект на приложение.
- [Актуализиране на регистрация на приложение – разрешения за API](https://docs.microsoft.com/graph/api/application-update) – тази статия ви показва как да актуализирате свойствата на обект на приложение.
- [Даване на съгласие](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) от администратор – За съгласие и съгласие от администратора по принцип изискваме администраторът изрично да даде съгласие.
- [RBAC (бета-версия)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – контейнер за управление на роли за единни дефиниции на роли и присвоявания на роли за доставчици на RBAC на Microsoft 365, които поддържат множество главници и множество обхвати в една задача на роля. Това е различно от *типа ресурс rbacApplication.* Microsoft Intune е пример за такъв доставчик на RBAC. Възложената роля в Intune може да има масив от главници и масив от групи с обхвати. **Това е в бета-версия, което означава, че все още е в процес на разработка и не се препоръчва за използване в производството.**
