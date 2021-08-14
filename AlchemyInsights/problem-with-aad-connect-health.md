---
title: Проблем с AAD Свързване изздрави
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
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923741"
---
# <a name="problem-with-aad-connect-health"></a>Проблем с AAD Свързване изздрави

- Уверете се, че сте упълномощени да изпълните операцията. Глобалните администратори имат достъп по подразбиране. Освен това можете да използвате контролата за [достъп, базирана на роли, за](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) да делегирате разрешение за регистрация на сътрудник.
- Уверете се, че задължителните крайни точки са разрешени и не са блокирани поради защитна стена. За подробности вижте [изисквания](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Регистрацията може да е неуспешна поради това, че изходящата комуникация е обект на SSL проверка от мрежовия слой.
- Уверете се, че сте проверили настройките за известия за Azure AD Свързване изцеднения. Прегледайте настройката си. Това [ръководство може](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) да ви помогне да разберете как да конфигурирате настройките за известия за Azure AD Свързване известия за изздравително състояние.
- За да научите повече за отчета за синхронизиране на Свързване из изтощиния и как да го изтеглите, вижте Отчет за синхронизиране [на ниво обект](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

За да отстраните неизправности с предупрежденията за Свързване изтръпване, следвайте ръководството за отстраняване на неизправности за [AAD Свързване](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Известия за свежестта на данните за изкачения и за често задавани въпроси вижте Често задавани въпроси за [инсталирането на AAD Свързване Из изтежност.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
