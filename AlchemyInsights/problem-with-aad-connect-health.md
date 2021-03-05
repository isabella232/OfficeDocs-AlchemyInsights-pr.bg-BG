---
title: Проблем със здравето на пад Connect
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480993"
---
# <a name="problem-with-aad-connect-health"></a>Проблем със здравето на пад Connect

- Уверете се, че сте упълномощени за извършване на операцията. Глобалните администратори имат достъп по подразбиране. Освен това можете да използвате [управление на достъпа, базирано на роли](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , за да предоставите разрешение за регистрация на представители.
- Уверете се, че задължителните крайни точки са разрешени и не са блокирани поради защитната стена. За подробности вижте [изисквания](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Регистрирането може да се провали поради изходящата комуникация, която се подлага на SSL проверка от мрежовия слой.
- Уверете се, че сте проверили настройките за известяване за Azure AD Connect Health. Моля, прегледайте настройката си. Това [ръководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) може да ви помогне да разберете как да конфигурирате настройките за известяване за известия за изправност на Azure ad Connect.
- За да научите повече за отчета за здравословно синхронизиране на пад-свързване и как да го изтеглите, вижте [отчет за синхронизиране на ниво на обект](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

За отстраняване на неизправности при свързване с пад на здравето, следвайте инструкциите [за отстраняване на неизправности за пад на известията за изправност на данните](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и често задавани въпроси вижте [Общи въпроси за инсталиране на здравето на пад](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
