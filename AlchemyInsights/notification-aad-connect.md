---
title: Свързване чрез пад на известията
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034916"
---
# <a name="notification-aad-connect"></a>Свързване чрез пад на известията

- Уверете се, че сте упълномощени за извършване на операцията. Глобалните администратори имат достъп по подразбиране. Освен това можете да използвате [управление на достъпа, базирано на роли](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , за да предоставите разрешение за регистрация на представители.
- Уверете се, че задължителните крайни точки са разрешени и не са блокирани поради защитната стена. За подробности вижте [изисквания](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Регистрирането може да се провали поради изходящата комуникация, която се подлага на SSL проверка от мрежовия слой.
- Уверете се, че сте проверили настройките за известяване за Azure AD Connect Health и прегледайте настройката си. За да разберете как да конфигурирате настройките за известия за уведомления за Azure AD Connect Health, вижте това [ръководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- За да научите повече за отчета за здравословно синхронизиране на пад-свързване и как да го изтеглите, вижте [отчет за синхронизиране на ниво на обект](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

За отстраняване на неизправности при известия за изправност на пад следвайте инструкциите [за отстраняване на неизправности за пад на известията за изправност на изправността](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и често задавани въпроси вижте [Общи въпроси за инсталиране на здравето на пад](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
