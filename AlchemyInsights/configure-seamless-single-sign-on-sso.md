---
title: Конфигуриране на безпроблемна еднократна идентификация (SSO)
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841400"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Конфигуриране на безпроблемна еднократна идентификация (SSO)

**Конфигуриране на приложения**

1. Би трябвало да получите стойностите от производителя на приложението. Можете ръчно да въведете стойностите или да качите файл с метаданни, за да извлечете стойността на полетата.
2. Много приложения вече са предварително конфигурирани за работа с Azure AD. Тези приложения са посочени в галерията с приложения, които можете да преглеждате, когато добавите приложение към своя клиент на Azure AD. Серията за бърз [Старт](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ви превежда през процеса.
3. За да създадете приложение, което не е в галерия, можете да щракнете върху **+ Създай свой собствен** бутон за приложение и да дадете име на вашата кандидатура.
    - По подразбиране той ще избере **интегриране на всяко друго приложение, което не можете да намерите в галерията** , което е правилната опция за приложенията, които не са галерия.
    - След като натиснете **Create** , след като сте поставили името на приложението, то ще създаде ново приложение, което не е в галерия Enterprise.
    - След това можете да се придвижите до **еднократна идентификация** под **управление** на това приложение и ще можете да видите различни техники за реализирането му във вашата среда.

**Конфигуриране на безпроблемно SSO за конкретно приложение**

За приложенията в галерията ще намерите подробни инструкции "стъпка по стъпка". За да получите достъп до стъпките, можете да прегледате списък с всички уроци за конфигуриране на приложението в [ръководствата за конфигуриране на приложението SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Конфигуриране на SAML-базиран SSO**

1. Бърз [Старт: Настройване на еднократна идентификация (SSO) на базата на SAML за приложение в Azure Active Directory (AZURE ad) клиент](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. За да научите повече за опцията, базирана на SAML, за еднократна идентификация, вижте [разбиране на базираните на SAML еднократна идентификация](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. За да научите повече за исканията за удостоверяване на SAML 2,0 и отговорите, които Azure Active Directory (Azure AD) поддържат за единични Sign-On (SSO), вижте [протокол за единична Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. За да научите как да създадете и конфигурирате еднократна идентификация (SSO) на SAML за вашето приложение в Azure Active Directory (Azure AD) с помощта на Microsoft Graph API, вижте конфигуриране на [еднократна идентификация за вашата заявка чрез Microsoft GRAPH API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. За да научите как Azure AD използва протокола SAML, вижте [как платформата за самоличност на Microsoft използва ПРОТОКОЛА SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Конфигуриране на маркери и рекламации**

1. [Как да: персонализирате искове, издадени в SAML маркер за корпоративни приложения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. За да научите как да конфигурирате искове с помощта на PowerShell, вижте [как да персонализирате искове, емитирани в маркери за конкретно приложение в клиент (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. За да научите как да конфигурирате претенциите по избор, вижте [как да: предоставяне на незадължителни искове за вашето приложение](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. За да научите как да използвате атрибути за разширение на схеми на справочен указател за изпращане на потребителски данни към приложения в претенции за маркери, вижте [използване на атрибути за разширение на схеми на справочен указател](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. За да научите как се конфигурират животи с маркери, вижте [конфигурируеми въплъщения за цял живот в Microsoft Identity Platform (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. Конфигуриране на правилата за [живот с маркери (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – в тази статия преминаваме през общ сценарий на политиката, който може да ви помогне да наложите нови правила за живота на маркера. В примера можете да научите как да създадете правило, което изисква потребителите да се удостоверят по-често във вашето уеб приложение.

**Отстраняване на неизправности при конфигуриране на SSO**

- За често задавани въпроси за Azure Active Directory безпроблемно един Sign-On (безшевни див), вижте [Azure Active Directory безшевни еднократна идентификация: често задавани въпроси](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- За информация за отстраняване на неизправности за често срещани проблеми, свързани с Azure Active Directory (Azure AD) безшевни единични Sign-On (безшевни SSO), вижте [отстраняване на неизправности в Azure Active Directory безпроблемно еднократна идентификация](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
