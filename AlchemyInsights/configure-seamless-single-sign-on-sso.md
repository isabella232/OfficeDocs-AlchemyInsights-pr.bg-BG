---
title: Конфигуриране на безпроблемна еднократна регистрация (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966026"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Конфигуриране на безпроблемна еднократна регистрация (SSO)

**Конфигуриране на приложения**

1. Трябва да получите стойностите от доставчика на приложението. Можете ръчно да въведете стойностите или да качите файл с метаданни, за да извлечете стойността на полетата.
2. Много приложения вече са предварително конфигурирани да работят с Azure AD. Тези приложения са изброени в галерията с приложения, които можете да преглеждате, когато добавяте приложение към вашия клиент на Azure AD. Серията ["Бързо започване"](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ще ви преобърне през процеса.
3. За да създадете приложение, което не е галерия, можете да щракнете **върху + Създаване** на собствен бутон "Приложение" и да дадете име на вашето приложение.
    - По подразбиране той ще избере Интегриране **на всяко друго** приложение, което не намирате в галерията, което е правилната опция за приложения, които не са галерия.
    - След като натиснете **Създай,** след като сте поставили името за приложението, то ще създаде ново корпоративно приложение, което не е галерия.
    - След това можете да отидете до **Еднократната** регистрация под **Управление** на това приложение и ще можете да видите различни техники за внедряването му във вашата среда.

**Конфигуриране на безпроблемна SSO за конкретно приложение**

За приложенията в галерията ще намерите подробни инструкции "стъпка по стъпка". За достъп до стъпките можете да прегледате списък с всички уроци за конфигуриране на приложения в уроците за [конфигуриране на приложението SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Конфигуриране на SSO, базиран на SAML**

1. [Бързо започване: Настройте базиран](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)на SAML еднократна регистрация (SSO) за приложение във вашия клиент на Azure Active Directory (Azure AD).
2. За да научите повече за базираната на SAML опция за еднократна регистрация, вижте Разбиране на еднократната еднократна регистрация, базирана [на SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. За да научите повече за заявките и отговорите за удостоверяване на SAML 2.0, които Azure Active Directory (Azure AD) поддържа за единичен Sign-On (SSO), [вж. Единичен Sign-On SAML протокол](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. За да научите как да създавате и конфигурирате базиран на SAML еднократна еднократна регистрация (SSO) за вашето приложение в Azure Active Directory (Azure AD) с помощта на API на Microsoft Graph, вижте Конфигуриране на еднократната еднократна регистрация, базирана на [SAML,](https://docs.microsoft.com/graph/application-saml-sso-configure-api)за вашето приложение с помощта на API на Microsoft Graph .
5. За да научите как Azure AD използва SAML протокола, вижте [Как Платформа за самоличност на Microsoft използва SAML протокола](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Конфигуриране на маркери и искове**

1. [Как да: персонализирате искове, издадени в saml маркера за корпоративни приложения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. За да научите как да конфигурирате искове с помощта на PowerShell, вижте Как да: Персонализиране на искове, излъчвани в маркери за конкретно приложение [в клиент (предварителен преглед).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. За да научите как да конфигурирате незадължителни искове, [вижте Как да: Предоставяне на незадължителни искове към вашето приложение.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. За да научите как да използвате атрибути за разширение на схема на справочна директория за изпращане на потребителски данни към приложения в искове с маркери, вижте Използване на атрибути за разширение [на схема на справочна директория в искове](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. За да научите как да конфигурирате животи на маркерите, вижте Конфигуриране на животи на [маркерите в Платформа за самоличност на Microsoft (предварителен преглед).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Конфигуриране на правила за живот на маркера (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – В тази статия ще преминем през общ сценарий на правила, който може да ви помогне да наложите нови правила за живот на маркера. В примера ще научите как да създадете правило, което изисква потребителите да удостоверяват по-често във вашето уеб приложение.

**Отстраняване на неизправности при SSO конфигурация**

- За често задавани въпроси за Azure Active Directory безпроблемна еднократна Sign-On (безпроблемна SSO) вижте Azure Active Directory Безпроблемно еднократната [регистрация: Често задавани въпроси.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- За отстраняване на неизправности с информация за често срещани проблеми по отношение на Azure Active Directory (Azure AD) – безпроблемна еднократна Sign-On (безпроблемна SSO), вижте [Отстраняване на неизправности Azure Active Directory безпроблемна](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)еднократна регистрация .
