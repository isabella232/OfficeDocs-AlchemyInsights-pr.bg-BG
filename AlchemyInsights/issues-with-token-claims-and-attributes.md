---
title: Проблеми с претенции за маркери и атрибути
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035833"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблеми с претенции за маркери и атрибути

**Актуализиране, конфигуриране или премахване на претенции за маркери**

1. Чрез използването на Azure Active Directory (Azure AD) можете да [персонализирате типа на иск за иск за роля](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) в маркера за отговор, който получавате, след като упълномощите приложение.
2. Разработчиците на приложения могат да използват незадължителни искове в своите приложения на Azure AD, за да укажат кои претенции желаят в маркерите, изпратени до тяхното приложение. За повече информация вижте [предоставяне на незадължителни искове за вашето приложение](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Конфигуриране на групови искове за приложения с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ако използвате безпроблемно еднократна идентификация във вашето приложение, вижте [Персонализиране на искове, издадени в SAML маркер за корпоративни приложения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Присвояване на атрибут за претенции**

1. За да конфигурирате правила за съпоставяне на искове с помощта на PowerShell, вижте [Персонализиране на искове, емитирани в маркери за конкретно приложение в клиент (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Атрибутите на справочното разширение на схемите предоставят начин да съхранявате допълнителни данни в Azure Active Directory в обекти на потребители и други обекти в указателя, като например групи, подробности за клиенти, основни услуги. За емитиране на искове за приложения могат да се използват само атрибути за разширение на потребителските обекти. [Използването на атрибути за разширение на схемата на справочен указател в искове](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) описва как да използвате атрибути за разширение на схеми на справочен указател за изпращане на потребителски данни към приложения в претенции за маркери.

За повече информация относно претенциите за маркери вижте:

- [Рекламации в маркерите на Access](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Вземания в id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Рекламации](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , които можете да ОЧАКВАТЕ в ИД маркери и маркери за достъп, издадени от AZURE ad B2C
- [Справка за претенции за SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
