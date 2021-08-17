---
title: SAML твърдения (маркери)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109229"
---
# <a name="saml-assertions-tokens"></a>SAML твърдения (маркери)

1. Маркерите за език за коректура за защита (SAML) са XML представяния на искове. По подразбиране маркерите на SAML Windows за комуникация (WCF) използва във федерирани сценарии на защита, се издават маркери. За повече информация вижте [SAML Маркери и искове](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Програмата Платформа за самоличност на Microsoft няколко типа маркери за защита при обработката на всеки поток на удостоверяване. [Препратката към исковете за маркери на SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) описва формата, характеристиките за защита и съдържанието на SAML 2,0 маркери.
3. Следвайте указанията в [конфигурируемите животи на маркерите в Платформа за самоличност на Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) за да разберете как да конфигурирате животите на маркерите.
4. Следвайте стъпките, описани в тази [статия, за](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) да разберете как да конфигурирате шифроването на SAML маркери на Azure AD.
5. В Azure AD можете да настроите опциите за подписване на сертификати и алгоритъма за подписване на сертификат. За повече информация вижте Разширени [опции за подписване на сертификат в маркера SAML за приложения на галерия в Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
