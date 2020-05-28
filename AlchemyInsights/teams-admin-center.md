---
title: Център за администриране на Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354077"
---
# <a name="teams-admin-center"></a>Център за администриране на Teams

Научете повече за управлението на Teams чрез [Центъра за администриране на Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ако не можете да получите достъп до Центъра за администриране на Teams, проверете следните неща:

- Уверете се, че сте позволили подходящи [IP адреси за Office 365, както и URL адреса ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всички устройства (защитна стена и т. н.) или в правилата за защитната стена на локалния ви компютър.
- Уверете се, че данните за влизане, които използвате за достъп до портала за администриране на Teams, съвпада с вашето потребителско име, посочено в [портала за администриране на Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ако потребителите не се показват в Центъра за администриране на Teams, проверете следното:

- Създали ли сте потребители или сте дали лицензи през последните 24 часа? Уверете се, че сте изчакали поне 24 часа, преди да отворите билет за поддръжка.
- Уверете се, че сте задали подходящи лицензи?
- Ако имате локална Active Directory, проверете дали [стойността на msRTCSIP-PrimaryUserAddress или SIP адрес в полето ProxyAddresses във вашата локална Active Directory е уникален и формат ът отговаря](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip: потребителско**име** на потребителя от центъра за администриране на [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ако възнамерявате да поддържате Skype за разполагане на бизнес сървър и потребители, които са удоманени локално и онлайн: следвайте **"Настройте хибрид с екипи и Онлайн на Skype за бизнеса"** във вашия Контролен панел на Skype за бизнес сървър и преместете потребителите онлайн.
