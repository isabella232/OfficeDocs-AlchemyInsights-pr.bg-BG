---
title: Проблеми с исковете и атрибутите на маркера
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012873"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблеми с исковете и атрибутите на маркера

**Актуализиране, конфигуриране или премахване на искове за маркери**

1. С помощта Azure Active Directory (Azure AD) [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) можете да персонализирате типа иск за искането за роля в маркера за отговор, който получавате, след като сте разрешили приложение.
2. Разработчиците на приложения могат да използват незадължителни искове в своите приложения на Azure AD, за да зададете какви претенции искат в маркерите, изпратени до приложението им. За повече информация вижте Предоставяне [на незадължителни искове към вашето приложение.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Конфигуриране на групови искове за приложения с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ако използвате безпроблемна еднократна регистрация във вашето приложение, вижте Персонализиране на искове, издадени [в маркера SAML за корпоративни приложения.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Съпоставяне на атрибути "Искове"**

1. За да конфигурирате правила за съпоставяне на искове с помощта на PowerShell, вижте Персонализиране на искове, излъчвани в маркери за [конкретно приложение в клиент (предварителен преглед).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Атрибутите за разширение на схемата на справочната схема предоставят начин за съхраняване на допълнителни данни в Azure Active Directory обекти на потребители и други обекти на справочника, като например групи, подробни данни за клиента, директори на услуги. Само атрибути за разширение на потребителски обекти могат да се използват за излъчване на искове към приложения. [Използването на атрибути за разширение на схемата на справочната](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) схема в искове описва как да използвате атрибути за разширение на справочна схема за изпращане на потребителски данни към приложения в искове за маркери.

За повече информация относно исковете за маркери вижте:

- [Искове в маркери за достъп](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Искове в id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Искове,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) които можете да очаквате в маркери за ИД и маркери за достъп, издадени от Azure AD B2C
- [Препратка към искове за маркери на SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
