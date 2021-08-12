---
title: Отстраняване на проблеми, свързани с безпроблемна еднократна еднократна регистрация (SSO) на базата на парола
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972813"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Отстраняване на проблеми, свързани с безпроблемна еднократна еднократна регистрация (SSO) на базата на парола

За да научите основите на SSO, базирано на парола, вижте Удостоверяване, базирано на [парола, Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Конфигуриране на SSO, базиран на парола**

1. [Конфигуриране на еднократната регистрация, базирана на парола](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – тази статия отива в по-подробна информация за опцията за SSO, базирана на парола. Ако приложението, което добавяте, изисква конфигурация по избор и трябва да използвате SSO, базиран на парола, тази статия е за вас.
2. [Конфигуриране на единичен знак, базиран](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) на парола, за приложения на място – Прокси сървърът на приложението поддържа няколко режима на еднократна регистрация. Влизането, базирано на парола, е предназначено за приложения, които използват комбинация от потребителско име/парола за удостоверяване. Когато конфигурирате влизане, базирано на парола за вашето приложение, вашите потребители трябва да впишат локалното приложение веднъж. След това Azure Active Directory съхранява информацията за влизане и автоматично я предоставя на приложението, когато вашите потребители имат отдалечен достъп до нея.
    - Би трябвало вече да сте публикували и тествали приложението си с прокси сървър за приложения. Ако не, следвайте стъпките в Публикуване на приложения с помощта на прокси сървъра за приложения на [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) след което продължете конфигурирането на SSO, базирано на парола, за приложенията за предварително използване.

За отстраняване на неизправности с SSO, базирани на пароли, вижте Отстраняване на [неизправности с еднократната влизане, базирано на парола, в Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
