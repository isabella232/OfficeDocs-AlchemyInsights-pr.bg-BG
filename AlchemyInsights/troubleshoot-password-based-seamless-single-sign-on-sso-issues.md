---
title: Отстраняване на проблеми с базирано на парола безпроблемно с еднократна идентификация (SSO)
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714679"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Отстраняване на проблеми с базирано на парола безпроблемно с еднократна идентификация (SSO)

За да научите основите на базиран на парола SSO, вижте [удостоверяване, базирано на парола с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Конфигуриране на базиран на парола SSO**

1. [Конфигуриране на базирани на парола еднократна идентификация](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -тази статия влиза в повече подробности за ОПЦИЯТА за SSO, базирана на парола. Ако приложението, което добавяте, изисква конфигурация по избор и трябва да използвате базирани на парола SSO, тази статия е за вас.
2. [Конфигуриране на базиран на парола еднократна идентификация за приложения на по-ниска база](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – прокси сървър на приложението поддържа няколко режима на еднократна идентификация. Базираното на парола влизане е предназначено за приложения, които използват комбинация от потребителско име и парола за удостоверяване. Когато конфигурирате влизане чрез парола за вашето приложение, вашите потребители трябва да влязат в локалното приложение еднократно. След това Azure Active Directory съхранява информацията за влизане и автоматично го предоставя на приложението, когато вашите потребители имат достъп до тях отдалечено.
    - Би трябвало вече да сте публикували и тествали приложението си чрез прокси сървър за приложения. Ако не е, следвайте стъпките в [публикуване на приложения чрез прокси сървър за приложения на AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) и след това продължете конфигурацията на базирани на парола SSO за приложения на по-програми.

За да отстраните базиран на парола SSO, вижте [отстраняване на неизправности при еднократна идентификация на базата на парола в AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
