---
title: Разрешаване на потребител да синхронизира личен акаунт със работния акаунт в Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813389"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Разрешаване на потребител да синхронизира личен акаунт със работния акаунт в Microsoft Edge

Уверете се, че отговаряте на следните критерии:

- Корпоративният щат роуминг е разрешен в центъра Azure Active Directory администриране, който изисква абонамент за Azure Active Directory Premium корпоративна мобилност + защита (EMS). За повече информация вижте Разрешаване [на корпоративния щат роуминг в Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Изпълнени са един или и двата критерия:
    - Услугата за защита на информацията на Azure е разрешена за вашия клиент. За подробности вижте [Активиране Azure Rights Management защита от Център за администриране на Microsoft 365](/azure/information-protection/activate-office365).
    - Функцията Azure Active Directory Enterprise State Roaming (ESR) е разрешена за всеки потребител или клиент. За повече информация вижте [Какво представлява роумингът в корпоративното състояние?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Ако AIP и ESR са забранени, съобщението за грешка информира потребителите, че синхронизирането не е налично за техните акаунти.
